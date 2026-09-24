# experiment-summary.json

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\experiment-summary.json`  
> **分类**: 配置 / 数据  
> **大小**: 6.4 KB  
> **最后修改**: 2026-09-24T08:04:03.034Z  

## 文件开头预览

```json
{
  "experimentName": "CoT with Chunks-First Prompt Caching",
  "date": "2026-09-24",
  "llmConfig": {
    "model": "deepseek-flash",
    "provider": "DeepSeek",
    "thinkingMode": "enabled",
    "cacheStrategy": "chunks-first (system prompt + examples ahead, question appended at end)",
    "apiEndpoint": "https://api.deepseek.com/chat/completions",
    "totalQuestions": 15,
    "questionIds": [
      "Z1-Q1","Z1-Q2","Z1-Q3","Z1-Q4",
      "Z2-Q1","Z2-Q2","Z2-Q3","Z2-Q4",
      "Z3-Q1","Z3-Q2","Z3-Q3",
      "Z4-Q1","Z4-Q2","Z4-Q3","Z4-Q4"
    ]
  },
  "aggregateMetrics": {
    "totalPromptTokens": 2405150,
    "totalCacheHitTokens": 2400512,
    "totalCacheMissTokens": 4638,
    "totalCompletionTokens": 157142,
    "totalReasoningTokens": 129853,
    "totalFinalAnswerTokens": 27289,
    "totalTokens": 2562292,
    "averageCacheHitRate": "99.81%",
    "totalElapsedTimeSeconds": 795.0,
    "averageTimePerQuestionSeconds": 53.0
  },
  "deepseekPricing": {
    "promptCacheHit": 0.36,
    "promptCacheMiss": 14.0,
    "completion": 14.0,
    "currency": "USD per Million tokens"
  },
  "costEstimate": {
    "cacheHitCost": "$0.8642",
    "cacheMissCost": "$0.0650",
    "completionCost": "$2.2000",
    "totalCostUSD": "$3.13",
    "notes": "Based on DeepSeek V3 pricing: cache hit=$0.36/MTok, cache miss=$14/MTok, completion=$14/MTok"
  },
  "perQuestionResults": [
    {
      "id": "Z1-Q1",
      "promptTokens": 160343,
      "cacheHit": 160128,
      "cacheMiss": 215,
      "completionTokens": 7233,
      "reasoningTokens": 5577,
```
