# call-0067-response.json

> **路径**: `snapshots\call-0067-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:58:36.497Z  

## 文件开头预览

```json
{
  "callId": "call-0067",
  "timestamp": "2026-09-24T10-58-35-964Z",
  "elapsed": 532,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3764,
      "completion_tokens": 2,
      "total_tokens": 3766,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3764
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "f25019bf-808e-4938-804d-eb1bb8d93c1b",
    "object": "chat.completion",
    "created": 1790247516,
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
      "prompt_tokens": 3764,
      "completion_tokens": 2,
      "total_tokens": 3766,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3764
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
