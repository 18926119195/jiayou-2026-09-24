# run-no-thinking.js

> **路径**: `cot对比实验\提高缓存命中率的实验\no-thinking-exp\run-no-thinking.js`  
> **分类**: 代码  
> **大小**: 4.7 KB  
> **最后修改**: 2026-09-24T06:24:25.543Z  

## 文件开头预览

```js
/**
 * no-thinking-exp · 关闭 thinking 对照实验推理脚本
 *
 * 与 ../run-cot-cache-exp.js 的唯一区别：
 *   - 使用 callLLM_NoThinking（reasoning_effort='none'，关闭 DeepThink）
 *   - 独立 API Key（no-thinking-exp/.env）
 *   - 输出写入 no-thinking-exp/<questionId>/ 子目录，不污染其他目录
 *
 * 用法（从 no-thinking-exp 文件夹内运行）：
 *   node run-no-thinking.js Z3-Q1
 *   node run-no-thinking.js Z3-Q2
 */

import fs from 'fs';
import path from 'path';
import { fileURLToPath } from 'url';
import { callLLM_NoThinking, LLM_BASE_URL, LLM_MODEL } from './llmClient-no-thinking.js';

const __dirname = path.dirname(fileURLToPath(import.meta.url));

// prompt 文件在父目录（提高缓存命中率的实验）中
const PROMPTS_DIR = path.join(__dirname, '..');

const questionId = process.argv[2];
if (!questionId) {
  console.error('用法: node run-no-thinking.js <questionId>');
  console.error('示例: node run-no-thinking.js Z3-Q1');
  process.exit(1);
}

const VALID_IDS = ['Z1-Q1','Z1-Q2','Z1-Q3','Z1-Q4','Z2-Q1','Z2-Q2','Z2-Q3','Z2-Q4',
                   'Z3-Q1','Z3-Q2','Z3-Q3','Z3-Q4','Z4-Q1','Z4-Q2','Z4-Q3','Z4-Q4'];
if (!VALID_IDS.includes(questionId)) {
  console.error(`未知 questionId: ${questionId}`);
  process.exit(1);
}

const QUESTION_MAP = {
  'Z3-Q1': '比较Pierre Janet、Freud、Karl Jaspers对无意识的理解有何异同？',
  'Z3-Q2': '精神分析如何处理精神病性结构？有哪些临床策略？',
};

// 输出写到 no-thinking-exp/<questionId>/ 子目录
const OUT_DIR = path.join(__dirname, questionId.replace('-', '_').toLowerCase());
if (!fs.existsSync(OUT_DIR)) {
  fs.mkdirSync(OUT_DIR, { recursive: true });
}

// 读取与 CoT 实验完全相同的 prompt（chunks-first 重排版）
const PROMPT_FILE = path.join(PROMPTS_DIR, `multipath-prompt-cot-${questionId}.txt`);
```
