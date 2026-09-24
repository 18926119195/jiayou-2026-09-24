# call-0619-response.json

> **路径**: `snapshots\call-0619-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:47.948Z  

## 文件开头预览

```json
{
  "callId": "call-0619",
  "timestamp": "2026-09-24T10-17-47-362Z",
  "elapsed": 582,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3866,
      "completion_tokens": 2,
      "total_tokens": 3868,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3866
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "9e1f69e2-7d47-4492-9b7d-b88f44c43e39",
    "object": "chat.completion",
    "created": 1790245067,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "NONE"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3866,
      "completion_tokens": 2,
      "total_tokens": 3868,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3866
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
