# call-0596-response.json

> **路径**: `snapshots\call-0596-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:45.941Z  

## 文件开头预览

```json
{
  "callId": "call-0596",
  "timestamp": "2026-09-24T10-17-45-347Z",
  "elapsed": 591,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3620,
      "completion_tokens": 2,
      "total_tokens": 3622,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3620
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "a2c8a955-d097-423f-9b3b-2779523132e0",
    "object": "chat.completion",
    "created": 1790245065,
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
      "prompt_tokens": 3620,
      "completion_tokens": 2,
      "total_tokens": 3622,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3620
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
