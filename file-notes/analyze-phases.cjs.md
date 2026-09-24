# analyze-phases.cjs

> **路径**: `analyze-phases.cjs`  
> **分类**: 代码  
> **大小**: 8.2 KB  
> **最后修改**: 2026-09-24T07:38:10.804Z  

## 文件开头预览

```cjs
const fs = require('fs');
const path = require('path');

// DeepSeek 定价 (CNY per 1M tokens)
const PRICING = {
  prompt_cache_miss: 1.0,
  prompt_cache_hit: 0.1,
  completion: 2.0
};

function analyzeQuestionPhases(questionDir) {
  const questionId = path.basename(questionDir);
  const files = fs.readdirSync(questionDir);
  const requestFiles = files.filter(f => f.endsWith('-request.json')).sort();
  const responseFiles = files.filter(f => f.endsWith('-response.json')).sort();
  
  // 识别粗筛阶段
  const coarseCallIds = [];
  const scoreCallIds = [];
  
  for (const reqFile of requestFiles) {
    const reqPath = path.join(questionDir, reqFile);
    const req = JSON.parse(fs.readFileSync(reqPath, 'utf8'));
    
    const isCoarse = req.promptPreview.includes('选出所有对回答这个问题可能有帮助的词');
    if (isCoarse) {
      coarseCallIds.push(req.callId);
    } else {
      scoreCallIds.push(req.callId);
    }
  }
  
  // 统计各阶段 token
  const coarseStats = { calls: 0, promptCacheMiss: 0, promptCacheHit: 0, completion: 0 };
  const scoreStats = { calls: 0, promptCacheMiss: 0, promptCacheHit: 0, completion: 0 };
  
  for (const resFile of responseFiles) {
    const resPath = path.join(questionDir, resFile);
    try {
      const res = JSON.parse(fs.readFileSync(resPath, 'utf8'));
      
      if (res.success && res.rawResponse && res.rawResponse.usage) {
        const usage = res.rawResponse.usage;
        const stats = coarseCallIds.includes(res.callId) ? coarseStats : scoreStats;
        
        stats.calls++;
        stats.promptCacheMiss += usage.prompt_cache_miss_tokens || 0;
        stats.promptCacheHit += usage.prompt_cache_hit_tokens || 0;
        stats.completion += usage.completion_tokens || 0;
      }
```
