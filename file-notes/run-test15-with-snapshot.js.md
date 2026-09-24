# run-test15-with-snapshot.js

> **路径**: `run-test15-with-snapshot.js`  
> **分类**: 代码  
> **大小**: 6.6 KB  
> **最后修改**: 2026-09-24T10:56:48.821Z  

## 文件开头预览

```js
#!/usr/bin/env node
/**
 * 在当前工作目录下运行完整的 15 问题推理流程，并快照所有 LLM 输入输出
 *
 * 功能：
 * 1. 在当前工作目录运行完整推理流程（阶段 2-5）
 * 2. 拦截所有 LLM 调用，快照每次的 prompt + response
 * 3. 保留所有中间数据文件
 * 4. 生成汇总报告
 *
 * 前置条件（必须在当前工作目录下存在）：
 *   - src/core/llmClient.js      （已内置 snapshot 功能）
 *   - src/core/pureTextTable.js
 *   - recall-nouns-llm.js
 *   - build-prompt-with-traceback.js
 *   - generate-multipath-prompt.js
 *   - run-reasoning.js
 *   - final-noun-index.json
 *   - test-questions.json
 *   - noun-blacklist.json
 *   - .env                      （含 API_KEY 等）
 *
 * 用法：
 *   node run-test15-with-snapshot.js
 *
 * 输出（全部写到当前工作目录）：
 *   snapshots/                         ← LLM 调用快照
 *     <QID>/
 *       call-NNNN-request.json
 *       call-NNNN-prompt.txt
 *       call-NNNN-response.json
 *       call-NNNN-output.txt
 *   noun-recall-results.json
 *   candidate-texts-for-llm.json
 *   material-traceback-map.json
 *   multipath-prompt-<QID>.txt   × 15
 *   reasoning-output-<QID>.json  × 15
 *   execution-summary.json
 */

import { execSync } from 'child_process';
import fs from 'fs';
import path from 'path';
import { fileURLToPath } from 'url';

const __dirname = path.dirname(fileURLToPath(import.meta.url));

// 当前工作目录 = 目标目录（由调用方决定）
const CWD = process.cwd();

```
