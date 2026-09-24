# run-cot-cache-exp.js

> **路径**: `cot对比实验\提高缓存命中率的实验\run-cot-cache-exp.js`  
> **分类**: 代码  
> **大小**: 5.1 KB  
> **最后修改**: 2026-09-24T07:09:35.416Z  

## 文件开头预览

```js
/**
 * 提高缓存命中率的实验 · 推理运行脚本
 *
 * 专门针对 "提高缓存命中率的实验" 文件夹内的 chunks-first 重排 prompt。
 * 所有中间产物和结果都写入本文件夹内，不污染父目录。
 *
 * 用法（从 "提高缓存命中率的实验" 文件夹内运行）：
 *   node run-cot-cache-exp.js Z3-Q1
 *   node run-cot-cache-exp.js Z3-Q2
 */

import fs from 'fs';
import path from 'path';
import { fileURLToPath } from 'url';
import { callLLM_CoT, LLM_BASE_URL, LLM_MODEL } from '../src-cot/llmClient-cot.js';

const __dirname = path.dirname(fileURLToPath(import.meta.url));

const questionId = process.argv[2];
if (!questionId) {
  console.error('用法: node run-cot-cache-exp.js <questionId>');
  console.error('示例: node run-cot-cache-exp.js Z3-Q1');
  process.exit(1);
}

// 验证 questionId 合法
const VALID_IDS = ['Z1-Q1','Z1-Q2','Z1-Q3','Z1-Q4','Z2-Q1','Z2-Q2','Z2-Q3','Z2-Q4',
                   'Z3-Q1','Z3-Q2','Z3-Q3','Z3-Q4','Z4-Q1','Z4-Q2','Z4-Q3','Z4-Q4'];
if (!VALID_IDS.includes(questionId)) {
  console.error(`未知 questionId: ${questionId}`);
  process.exit(1);
}

// 问题文本映射（从 prompt 文件内提取）
const QUESTION_MAP = {
  'Z3-Q1': '比较Pierre Janet、Freud、Karl Jaspers对无意识的理解有何异同？',
  'Z3-Q2': '精神分析如何处理精神病性结构？有哪些临床策略？',
};

// 输出目录
const OUT_DIR = path.join(__dirname, questionId.replace('-', '_').toLowerCase());
// 示例：Z3-Q1 → z3_q1/  Z3-Q2 → z3_q2/

if (!fs.existsSync(OUT_DIR)) {
  fs.mkdirSync(OUT_DIR, { recursive: true });
}

// Prompt 文件路径（chunks-first 重排版，在本文件夹内）
const PROMPT_FILE = path.join(__dirname, `multipath-prompt-cot-${questionId}.txt`);
if (!fs.existsSync(PROMPT_FILE)) {
```
