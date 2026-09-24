# llmClient-cot.js

> **路径**: `cot对比实验\src-cot\llmClient-cot.js`  
> **分类**: 代码  
> **大小**: 3.9 KB  
> **最后修改**: 2026-09-24T06:24:25.557Z  

## 文件开头预览

```js
/**
 * CoT 对比实验专用 LLM 客户端
 *
 * 与 src/core/llmClient.js 的唯一区别：
 *   reasoning_effort: 'none'  →  'high' + thinking type=enabled
 *
 * 用于实验组一（CoT）的名词召回和推理阶段。
 */

import fs from 'fs';
import path from 'path';

function loadDotEnv() {
  const envPath = path.join(process.cwd(), '.env');
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
    if (!(key in process.env)) process.env[key] = value;
  }
}

loadDotEnv();

export const LLM_BASE_URL = process.env.LLM_BASE_URL || 'https://api.deepseek.com';
export const LLM_MODEL = process.env.LLM_MODEL || 'deepseek-flash';   // DeepSeek-V4.1-Flash（默认即 Flash V4，不再回退到 V4-Pro）
export const LLM_API_KEY = process.env.LLM_API_KEY || process.env.OPENAI_API_KEY || '';

export const DEFAULT_MAX_TOKENS = 384000;

/**
 * 对齐官网 chat.deepseek.com 默认行为（基于 Flash V4）：
 *   temperature = 0.6（Flash V4 默认温度）
 *   max_tokens = 384000（Flash V4 上限输出）
 *   reasoning_effort = 'high'（DeepThink 模式）
 *   thinking = { type: 'enabled' }
 *
 * 注：之前默认是 'deepseek-v4-pro'，已统一改为 'deepseek-flash'（Flash V4），
 *    与 .env 中的 LLM_MODEL 配置保持一致，且更经济（Flash 比 Pro 便宜约 4 倍）。
 */

if (!LLM_API_KEY) {
```
