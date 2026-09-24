# test-cache-warmup-z3q2.js

> **路径**: `test-cache-warmup-z3q2.js`  
> **分类**: 代码  
> **大小**: 4.2 KB  
> **最后修改**: 2026-09-24T12:10:22.302Z  

## 文件开头预览

```js
/**
 * 缓存预热测试：第一批全量 + 后续递减分批
 * 
 * 策略：
 * 1. 第1批：全量名词（1-N），建立完整缓存
 * 2. 第2批：前 N/2 个名词 → 命中第1批前缀缓存
 * 3. 第3批：前 N/4 个名词 → 命中第2批前缀缓存
 * ...
 * 
 * 测试问题：Z3-Q2
 * API Key: sk-***REDACTED***
 */

import fs from 'fs';
import path from 'path';

// 临时覆盖 API key（仅本次测试）
process.env.DEEPSEEK_API_KEY = 'sk-***REDACTED***';

import { callLLM } from './src/core/llmClient.js';

const NOUN_INDEX_PATH = path.join(process.cwd(), 'final-noun-index.json');
const QUESTIONS_PATH = path.join(process.cwd(), 'test-questions.json');
const OUTPUT_PATH = path.join(process.cwd(), 'cache-warmup-test-z3q2.json');

console.log('=== 缓存预热测试（递减分批策略）===\n');

const nounIndex = JSON.parse(fs.readFileSync(NOUN_INDEX_PATH, 'utf-8'));
const questions = JSON.parse(fs.readFileSync(QUESTIONS_PATH, 'utf-8'));
const question = questions.find(q => q.id === 'Z3-Q2');

if (!question) {
  console.error('未找到 Z3-Q2');
  process.exit(1);
}

console.log(`问题: ${question.question}`);
console.log(`全量名词数: ${nounIndex.nouns.length}\n`);

function buildCoarsePrompt(questionText, nounList) {
  const list = nounList.map((n, i) => `【【${i + 1}】】${n.surface}`).join('\n');
  return `问题: ${questionText}

从下列名词中，选出所有对回答这个问题可能有帮助的词。只回答相关词的机器符号，例如：【【1】】【【5】】【【17】】
如果没有任何相关词，回答：NONE

词语列表：
${list}

相关词编号：`;
```
