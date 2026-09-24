# check-cache-hit-by-stage.js

> **路径**: `check-cache-hit-by-stage.js`  
> **分类**: 代码  
> **大小**: 2.6 KB  
> **最后修改**: 2026-09-24T11:08:15.459Z  

## 文件开头预览

```js
import fs from 'fs';
import path from 'path';

const dir = path.join(process.cwd(), 'snapshots');
const files = fs.readdirSync(dir).filter(f => f.endsWith('-request.json'));

function classify(promptText) {
  if (!promptText) return 'unknown';
  // 粗筛特征：包含"只回答相关词的机器符号"和"如果没有任何相关词，回答：NONE"
  if (promptText.includes('只回答相关词的机器符号') || promptText.includes('如果没有任何相关词，回答：NONE')) {
    return 'coarse';
  }
  // 精打特征：包含"请按重要程度打分"
  if (promptText.includes('请按重要程度打分') || promptText.includes('81-100 核心概念')) {
    return 'score';
  }
  // 推理特征：包含"材料："和"(命中: "（缓存命中率标记）
  if (promptText.includes('材料：') && promptText.includes('(命中: ')) {
    return 'reasoning';
  }
  return 'other';
}

const stageStats = {};

for (const f of files) {
  const callId = f.replace('-request.json', '');
  const reqPath = path.join(dir, f);
  const resPath = path.join(dir, `${callId}-response.json`);
  if (!fs.existsSync(resPath)) continue;

  let reqData, resData;
  try {
    reqData = JSON.parse(fs.readFileSync(reqPath, 'utf-8'));
    resData = JSON.parse(fs.readFileSync(resPath, 'utf-8'));
  } catch {
    continue;
  }

  const usage = resData.response?.usage;
  if (!usage) continue;

  const promptText = reqData.fullPrompt || reqData.promptPreview || '';

  const stage = classify(promptText);
  const hit = usage.prompt_cache_hit_tokens || 0;
  const miss = usage.prompt_cache_miss_tokens || 0;

  if (!stageStats[stage]) {
    stageStats[stage] = { calls: 0, hit: 0, miss: 0 };
```
