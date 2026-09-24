# llmClient-no-thinking.js

> **路径**: `cot对比实验\提高缓存命中率的实验\no-thinking-exp\llmClient-no-thinking.js`  
> **分类**: 代码  
> **大小**: 3.2 KB  
> **最后修改**: 2026-09-24T06:24:25.537Z  

## 文件开头预览

```js
/**
 * no-thinking-exp · 关闭 thinking 对照实验 LLM 客户端
 *
 * 与 src-cot/llmClient-cot.js 的唯一区别：
 *   reasoning_effort: 'none'  （关闭 DeepThink）
 *   thinking: { type: 'disabled' }
 *
 * 使用独立 API Key（sk-9541402e22d64ac...），不影响主实验账号。
 */

import fs from 'fs';
import path from 'path';
import { fileURLToPath } from 'url';

function loadDotEnv(dir) {
  const envPath = path.join(dir, '.env');
  if (!fs.existsSync(envPath)) return;
  const content = fs.readFileSync(envPath, 'utf-8');
  for (const line of content.split(/\r?\n/)) {
    const trimmed = line.trim();
    if (!trimmed || trimmed.startsWith('#')) continue;
    const eq = trimmed.indexOf('=');
    if (eq === -1) continue;
    const key = trimmed.slice(0, eq).trim();
    let value = trimmed.slice(eq + 1).trim();
    if ((value.startsWith('"') && value.endsWith('"')) || (value.startsWith("'") && value.endsWith("'"))) {
      value = value.slice(1, -1);
    }
    // 强制覆盖（对照实验用独立 Key）
    process.env[key] = value;
  }
}

// 优先加载本目录的 .env（独立 API Key）
const __dirname = path.dirname(fileURLToPath(import.meta.url));
loadDotEnv(__dirname);

export const LLM_BASE_URL = process.env.LLM_BASE_URL || 'https://api.deepseek.com';
export const LLM_MODEL    = process.env.LLM_MODEL    || 'deepseek-flash';
export const LLM_API_KEY  = process.env.LLM_API_KEY  || '';
export const DEFAULT_MAX_TOKENS = 384000;

if (!LLM_API_KEY) {
  console.error('[NoThinking] 缺少 API 密钥：请在 .env 中设置 LLM_API_KEY');
}

/**
 * 关闭 thinking 版 LLM 调用
 * deepseek-flash + reasoning_effort='none' + thinking type=disabled
 */
```
