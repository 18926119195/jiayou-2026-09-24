# token-cost-report.json

> **路径**: `问题一\runs\2026-09-23-cache-test-rerun-remainder\token-cost-report.json`  
> **分类**: 配置 / 数据  
> **大小**: 118.7 KB  
> **最后修改**: 2026-09-24T07:24:46.040Z  

## 文件开头预览

```json
{
  "summary": {
    "totalQuestions": 13,
    "totalCalls": 690,
    "totalTokens": {
      "promptCacheMiss": 255654,
      "promptCacheHit": 2189285,
      "completion": 99835,
      "totalPrompt": 2444939,
      "total": 2544774
    },
    "totalCost": 0.6742525
  },
  "details": [
    {
      "questionId": "Z1-Q2",
      "callCount": 99,
      "tokens": {
        "promptCacheMiss": 40597,
        "promptCacheHit": 312576,
        "completion": 15417,
        "totalPrompt": 353173,
        "total": 368590
      },
      "cost": {
        "cacheMiss": 0.040597,
        "cacheHit": 0.0312576,
        "completion": 0.030834,
        "total": 0.1026886
      },
      "callDetails": [
        {
          "callId": "call-0001",
          "cacheMiss": 186,
          "cacheHit": 3456,
          "completion": 57,
          "totalPrompt": 3642
        },
        {
          "callId": "call-0002",
          "cacheMiss": 209,
          "cacheHit": 3456,
          "completion": 73,
          "totalPrompt": 3665
        },
        {
          "callId": "call-0003",
          "cacheMiss": 136,
          "cacheHit": 3456,
          "completion": 37,
```
