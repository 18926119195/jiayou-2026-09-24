# llmClient.js

> **路径**: `src\core\llmClient.js`  
> **分类**: 代码  
> **大小**: 5.9 KB  
> **最后修改**: 2026-09-24T10:21:27.493Z  

## 文件开头预览

```js
import fs from 'fs';
import path from 'path';
import { fileURLToPath } from 'url';

const __dirname = path.dirname(fileURLToPath(import.meta.url));

// 原始 LLM 客户端配置
export const LLM_BASE_URL = process.env.LLM_BASE_URL || 'https://api.deepseek.com';
export const LLM_MODEL = process.env.LLM_MODEL || 'deepseek-flash';
export const LLM_API_KEY = process.env.LLM_API_KEY || process.env.DEEPSEEK_API_KEY;

if (!LLM_API_KEY) {
  console.error('错误: 缺少 LLM_API_KEY 或 DEEPSEEK_API_KEY 环境变量');
  process.exit(1);
}

const SNAPSHOT_DIR = path.join(process.cwd(), 'snapshots');
let callCounter = 0;

export async function callLLM(prompt, options = {}) {
  callCounter++;
  const callId = `call-${String(callCounter).padStart(4, '0')}`;
  const timestamp = new Date().toISOString().replace(/[:.]/g, '-');

  const maxTokens = options.maxTokens || 32768;
  const maxRetries = options.maxRetries ?? 3;
  const baseRetryDelayMs = options.retryDelayMs ?? 2000;

  console.log(`\n[${callId}] LLM 调用开始...`);
  console.log(`  Prompt 长度: ${prompt.length} 字符`);
  console.log(`  Max tokens: ${maxTokens}`);
  console.log(`  重试策略: 最多 ${maxRetries} 次，初始退避 ${baseRetryDelayMs}ms（指数退避）`);

  // 保存请求快照
  const requestSnapshot = {
    callId,
    timestamp,
    promptLength: prompt.length,
    promptPreview: prompt.substring(0, 500) + (prompt.length > 500 ? '...' : ''),
    fullPrompt: prompt,
    options: { ...options, maxRetries, baseRetryDelayMs },
  };
  fs.writeFileSync(
    path.join(SNAPSHOT_DIR, `${callId}-request.json`),
    JSON.stringify(requestSnapshot, null, 2),
    'utf-8'
  );
  fs.writeFileSync(
    path.join(SNAPSHOT_DIR, `${callId}-prompt.txt`),
    prompt,
```
