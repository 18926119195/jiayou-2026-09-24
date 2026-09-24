# call-0236-response.json

> **路径**: `snapshots\call-0236-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:15:58.649Z  

## 文件开头预览

```json
{
  "callId": "call-0236",
  "timestamp": "2026-09-24T10-15-57-902Z",
  "elapsed": 743,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【11】】【【140】】【【169】】【【172】】【【300】】【【301】】",
    "usage": {
      "prompt_tokens": 3730,
      "completion_tokens": 25,
      "total_tokens": 3755,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3730
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "2bdc36c2-1d4a-41d3-aa46-a69765aab1b8",
    "object": "chat.completion",
    "created": 1790244958,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【11】】【【140】】【【169】】【【172】】【【300】】【【301】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3730,
      "completion_tokens": 25,
      "total_tokens": 3755,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3730
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
