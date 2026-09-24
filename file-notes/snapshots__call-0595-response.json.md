# call-0595-response.json

> **路径**: `snapshots\call-0595-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:45.904Z  

## 文件开头预览

```json
{
  "callId": "call-0595",
  "timestamp": "2026-09-24T10-17-45-332Z",
  "elapsed": 570,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3385,
      "completion_tokens": 2,
      "total_tokens": 3387,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3385
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "bb2f021e-4b93-4487-bf25-e07358aa5ec6",
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
      "prompt_tokens": 3385,
      "completion_tokens": 2,
      "total_tokens": 3387,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3385
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
