# call-0669-response.json

> **路径**: `snapshots\call-0669-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:59.793Z  

## 文件开头预览

```json
{
  "callId": "call-0669",
  "timestamp": "2026-09-24T10-17-58-986Z",
  "elapsed": 804,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3486,
      "completion_tokens": 2,
      "total_tokens": 3488,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3486
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "c9ca4ec4-f0a2-4852-9174-9f546b69d61a",
    "object": "chat.completion",
    "created": 1790245079,
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
      "prompt_tokens": 3486,
      "completion_tokens": 2,
      "total_tokens": 3488,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3486
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
