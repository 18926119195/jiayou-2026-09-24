# recall-nouns-llm.js

> **路径**: `recall-nouns-llm.js`  
> **分类**: 代码  
> **大小**: 23.5 KB  
> **最后修改**: 2026-09-24T09:48:36.173Z  

## 文件开头预览

```js
/**
 * 基于词表拓扑链的召回引擎（两步粗筛 + 精打分架构）
 *
 * 流程：
 * 1. 粗筛（LLM 1 轮）：快速判断"是否相关"，每批输入【【N】】词语，只回【【N】】列表或 NONE
 * 2. 精打（LLM 2 轮）：只对粗筛 YES 的词打分，每批输入【【N】】词语，只回 JSON 数组
 * 3. 高分词 → 构建拓扑链 → 映射 bookKey → ChunkKey 去重 → 召回原文
 *
 * LLM 调用统一走 src/core/llmClient.js（DeepSeek，deepseek-chat，thinking 强制关闭）。
 *
 * 用法：
 *   node recall-nouns-llm.js                      # 所有问题
 *   node recall-nouns-llm.js Z1-Q1 Z1-Q2           # 指定问题ID
 *   NOUN_BATCH_SIZE=500 node recall-nouns-llm.js   # 粗筛批次大小（默认500）
 */

import fs from 'fs';
import path from 'path';
import { callLLM, LLM_BASE_URL, LLM_MODEL } from './src/core/llmClient.js';
import { atomSearchText, isRetrievableAtom } from './src/core/pureTextTable.js';

// ============ 配置（环境变量覆盖）============
const DOCUVERSE_PATH = process.env.DOCUVERSE_PATH || 'C:\\Users\\Administrator\\Desktop\\docuverse_cartographies_squizoanalythiques_Fe_lix_Guattari_1789114122714.docuverse.json';
const NOUN_INDEX_PATH = process.env.NOUN_INDEX_PATH || path.join(process.cwd(), 'final-noun-index.json');
const QUESTIONS_PATH = process.env.QUESTIONS_PATH || path.join(process.cwd(), 'test-questions.json');
const OUTPUT_PATH = process.env.OUTPUT_PATH || path.join(process.cwd(), 'noun-recall-results.json');

// ============ 黑名单过滤（送给LLM之前；不动名词表）============
const BLACKLIST_PATH = process.env.NOUN_BLACKLIST_PATH || path.join(process.cwd(), 'noun-blacklist.json');
const FILTER_BLACKLIST = (process.env.FILTER_BLACKLIST || '1') === '1'; // 默认开启，设为 0 可关闭

const CONCURRENCY = parseInt(process.env.LLM_CONCURRENCY || '8', 10);
const TOPOLOGY_WINDOW = parseInt(process.env.TOPOLOGY_WINDOW || '2', 10);
const QUESTION_IDS = process.argv.slice(2).length
  ? process.argv.slice(2)
  : (process.env.QUESTION_IDS || '').split(',').filter(Boolean);

// ============ Token 预算控制（对齐 s1-llm-fill.js）============
const CHARS_PER_TOKEN = 3.5;
const MAX_PROMPT_TOKENS = 2500; // 每批 prompt 最多 2500 tokens（预算分批依据，不变）
const MAX_COARSE_OUTPUT_TOKENS = 32768; // 粗筛输出上限（V4-Flash: 384K，设为 32K 安全阈值）
const MAX_SCORE_OUTPUT_TOKENS = 32768; // 精打输出上限（V4-Flash: 384K，设为 32K 安全阈值）

function estimatePromptTokens(text) {
  return Math.ceil(text.length / CHARS_PER_TOKEN);
}

console.log(`LLM: ${LLM_BASE_URL} model=${LLM_MODEL} thinking=disabled`);

// ============ 加载数据 ============
```
