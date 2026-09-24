# reorder-prompts-for-cache.js

> **路径**: `cot对比实验\提高缓存命中率的实验\reorder-prompts-for-cache.js`  
> **分类**: 代码  
> **大小**: 4.1 KB  
> **最后修改**: 2026-09-24T06:24:25.403Z  

## 文件开头预览

```js
/**
 * 提升缓存命中率实验：将 15 个全量 prompt 中的"问题头+要求+格式+规范+策略"
 * 全部移到末尾、把"全量材料"区块挪到最前面。
 *
 * 约束：字字不差，仅换位置（用 indexOf 找到【【全量材料】】的字节位置，按字节切两段、再反向拼接）。
 *
 * 缓存原理：
 *   DeepSeek API 的 prefix cache 命中是从 prompt 开头算起的连续相同前缀。
 *   原顺序：[问题头 + 1446 chunks]   → 每个问题开头不同，cache 命中率=0%
 *   新顺序：[1446 chunks + 问题头]   → 1446 chunks 部分在 15 个问题间完全一致，
 *                                      第二个问题开始就能命中前面 165k tokens 的前缀
 */

import fs from 'fs';
import path from 'path';
import { fileURLToPath } from 'url';

const __dirname = path.dirname(fileURLToPath(import.meta.url));
const SRC_DIR = path.resolve(__dirname, '..');
const OUT_DIR = __dirname;
const LOG_PATH = path.join(__dirname, '_reorder_result.txt');

const MARKER = '【【全量材料】】';

const QIDS = [
  'Z1-Q1', 'Z1-Q2', 'Z1-Q3', 'Z1-Q4',
  'Z2-Q1', 'Z2-Q2', 'Z2-Q3', 'Z2-Q4',
  'Z3-Q1', 'Z3-Q2', 'Z3-Q3',
  'Z4-Q1', 'Z4-Q2', 'Z4-Q3', 'Z4-Q4',
];

const lines = [];
const log = (msg) => { console.log(msg); lines.push(msg); };

let totalSrcBytes = 0;
let totalOutBytes = 0;

log('==== CoT 对比实验：缓存命中率优化版（chunks 前置）====');
log(`SRC: ${SRC_DIR}`);
log(`OUT: ${OUT_DIR}`);
log('');

for (const qid of QIDS) {
  const srcPath = path.join(SRC_DIR, `multipath-prompt-cot-${qid}.txt`);
  const outPath = path.join(OUT_DIR, `multipath-prompt-cot-${qid}.txt`);

  if (!fs.existsSync(srcPath)) {
    log(`[FAIL] ${qid}: source not found at ${srcPath}`);
    continue;
  }
```
