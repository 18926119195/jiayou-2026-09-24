# call-0482-response.json

> **路径**: `snapshots\call-0482-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:03.463Z  

## 文件开头预览

```json
{
  "callId": "call-0482",
  "timestamp": "2026-09-24T10-17-02-950Z",
  "elapsed": 510,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3674,
      "completion_tokens": 2,
      "total_tokens": 3676,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3674
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "d79fa824-3499-4143-a336-82245780d5c7",
    "object": "chat.completion",
    "created": 1790245023,
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
      "prompt_tokens": 3674,
      "completion_tokens": 2,
      "total_tokens": 3676,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3674
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
