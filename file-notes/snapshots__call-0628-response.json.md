# call-0628-response.json

> **路径**: `snapshots\call-0628-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:48.290Z  

## 文件开头预览

```json
{
  "callId": "call-0628",
  "timestamp": "2026-09-24T10-17-47-946Z",
  "elapsed": 341,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 1687,
      "completion_tokens": 2,
      "total_tokens": 1689,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 1687
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "3e8a78d0-0f76-4f48-a11e-19a36043c252",
    "object": "chat.completion",
    "created": 1790245068,
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
      "prompt_tokens": 1687,
      "completion_tokens": 2,
      "total_tokens": 1689,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 1687
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
