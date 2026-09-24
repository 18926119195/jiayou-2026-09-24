# analyze-token-cost.cjs

> **路径**: `analyze-token-cost.cjs`  
> **分类**: 代码  
> **大小**: 7.1 KB  
> **最后修改**: 2026-09-24T07:23:40.466Z  

## 文件开头预览

```cjs
const fs = require('fs');
const path = require('path');

// DeepSeek 定价 (CNY per 1M tokens)
const PRICING = {
  prompt_cache_miss: 1.0,  // 输入缓存未命中
  prompt_cache_hit: 0.1,   // 输入缓存命中
  completion: 2.0          // 输出
};

function analyzeQuestion(questionDir) {
  const files = fs.readdirSync(questionDir);
  const responseFiles = files.filter(f => f.endsWith('-response.json'));
  
  let totalPromptCacheMiss = 0;
  let totalPromptCacheHit = 0;
  let totalCompletion = 0;
  const callDetails = [];
  
  for (const file of responseFiles) {
    const filePath = path.join(questionDir, file);
    try {
      const data = JSON.parse(fs.readFileSync(filePath, 'utf8'));
      
      if (data.success && data.rawResponse && data.rawResponse.usage) {
        const usage = data.rawResponse.usage;
        const cacheMiss = usage.prompt_cache_miss_tokens || 0;
        const cacheHit = usage.prompt_cache_hit_tokens || 0;
        const completion = usage.completion_tokens || 0;
        
        totalPromptCacheMiss += cacheMiss;
        totalPromptCacheHit += cacheHit;
        totalCompletion += completion;
        
        callDetails.push({
          callId: data.callId,
          cacheMiss,
          cacheHit,
          completion,
          totalPrompt: cacheMiss + cacheHit
        });
      }
    } catch (err) {
      console.error(`Error reading ${file}:`, err.message);
    }
  }
  
  // 计算费用 (CNY)
  const costCacheMiss = (totalPromptCacheMiss / 1_000_000) * PRICING.prompt_cache_miss;
  const costCacheHit = (totalPromptCacheHit / 1_000_000) * PRICING.prompt_cache_hit;
```
