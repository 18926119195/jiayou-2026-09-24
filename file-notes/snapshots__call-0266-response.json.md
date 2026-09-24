# call-0266-response.json

> **路径**: `snapshots\call-0266-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:16:01.049Z  

## 文件开头预览

```json
{
  "callId": "call-0266",
  "timestamp": "2026-09-24T10-16-00-624Z",
  "elapsed": 421,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 1681,
      "completion_tokens": 2,
      "total_tokens": 1683,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 1681
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "95fa4a88-654b-4133-a328-b1d82997e0f0",
    "object": "chat.completion",
    "created": 1790244960,
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
      "prompt_tokens": 1681,
      "completion_tokens": 2,
      "total_tokens": 1683,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 1681
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
