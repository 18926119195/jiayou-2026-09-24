# call-0377-response.json

> **路径**: `snapshots\call-0377-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:16:35.822Z  

## 文件开头预览

```json
{
  "callId": "call-0377",
  "timestamp": "2026-09-24T10-16-35-239Z",
  "elapsed": 580,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3801,
      "completion_tokens": 2,
      "total_tokens": 3803,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3801
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "649246e2-be7e-43c0-bdd9-55d50c8aaf9f",
    "object": "chat.completion",
    "created": 1790244995,
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
      "prompt_tokens": 3801,
      "completion_tokens": 2,
      "total_tokens": 3803,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3801
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
