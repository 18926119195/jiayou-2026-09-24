# call-0462-response.json

> **路径**: `snapshots\call-0462-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:01.520Z  

## 文件开头预览

```json
{
  "callId": "call-0462",
  "timestamp": "2026-09-24T10-17-01-197Z",
  "elapsed": 319,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3735,
      "completion_tokens": 2,
      "total_tokens": 3737,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3735
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "e5e676e6-ca3f-4e5d-9df2-578696b988fd",
    "object": "chat.completion",
    "created": 1790245021,
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
      "prompt_tokens": 3735,
      "completion_tokens": 2,
      "total_tokens": 3737,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3735
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
