# call-0251-response.json

> **路径**: `snapshots\call-0251-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:16:00.138Z  

## 文件开头预览

```json
{
  "callId": "call-0251",
  "timestamp": "2026-09-24T10-15-59-135Z",
  "elapsed": 999,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3532,
      "completion_tokens": 2,
      "total_tokens": 3534,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3532
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "4be57d70-1439-4e91-abac-e032de7cb5ce",
    "object": "chat.completion",
    "created": 1790244959,
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
      "prompt_tokens": 3532,
      "completion_tokens": 2,
      "total_tokens": 3534,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3532
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
