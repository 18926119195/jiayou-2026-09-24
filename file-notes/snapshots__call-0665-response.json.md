# call-0665-response.json

> **路径**: `snapshots\call-0665-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:17:59.344Z  

## 文件开头预览

```json
{
  "callId": "call-0665",
  "timestamp": "2026-09-24T10-17-58-845Z",
  "elapsed": 496,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【23】】【【318】】",
    "usage": {
      "prompt_tokens": 3678,
      "completion_tokens": 9,
      "total_tokens": 3687,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3678
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "f88f5ba7-1203-4c6a-963e-68d1f58d653b",
    "object": "chat.completion",
    "created": 1790245079,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【23】】【【318】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3678,
      "completion_tokens": 9,
      "total_tokens": 3687,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3678
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
