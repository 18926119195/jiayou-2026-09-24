# call-0648-response.json

> **路径**: `snapshots\call-0648-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:58.192Z  

## 文件开头预览

```json
{
  "callId": "call-0648",
  "timestamp": "2026-09-24T10-17-57-635Z",
  "elapsed": 553,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3945,
      "completion_tokens": 2,
      "total_tokens": 3947,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3945
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "d1eccf5c-0750-4734-a3e3-13f7669b195f",
    "object": "chat.completion",
    "created": 1790245077,
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
      "prompt_tokens": 3945,
      "completion_tokens": 2,
      "total_tokens": 3947,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3945
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
