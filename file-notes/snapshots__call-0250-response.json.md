# call-0250-response.json

> **路径**: `snapshots\call-0250-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:15:59.851Z  

## 文件开头预览

```json
{
  "callId": "call-0250",
  "timestamp": "2026-09-24T10-15-59-107Z",
  "elapsed": 742,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【292】】",
    "usage": {
      "prompt_tokens": 3254,
      "completion_tokens": 5,
      "total_tokens": 3259,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3254
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "31f09b36-07b7-4d6c-96ab-78963e01783d",
    "object": "chat.completion",
    "created": 1790244959,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【292】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3254,
      "completion_tokens": 5,
      "total_tokens": 3259,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3254
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
