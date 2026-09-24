# call-0662-response.json

> **路径**: `snapshots\call-0662-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:59.154Z  

## 文件开头预览

```json
{
  "callId": "call-0662",
  "timestamp": "2026-09-24T10-17-58-482Z",
  "elapsed": 669,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3677,
      "completion_tokens": 2,
      "total_tokens": 3679,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3677
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "a0eaaf2e-83ac-4fd7-b488-a9a50761e48b",
    "object": "chat.completion",
    "created": 1790245078,
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
      "prompt_tokens": 3677,
      "completion_tokens": 2,
      "total_tokens": 3679,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3677
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
