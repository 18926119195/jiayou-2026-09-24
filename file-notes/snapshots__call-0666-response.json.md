# call-0666-response.json

> **路径**: `snapshots\call-0666-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:59.804Z  

## 文件开头预览

```json
{
  "callId": "call-0666",
  "timestamp": "2026-09-24T10-17-58-889Z",
  "elapsed": 913,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3664,
      "completion_tokens": 2,
      "total_tokens": 3666,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3664
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "4297ec06-418d-451a-9ff6-aede14afc0b9",
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
      "prompt_tokens": 3664,
      "completion_tokens": 2,
      "total_tokens": 3666,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3664
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
