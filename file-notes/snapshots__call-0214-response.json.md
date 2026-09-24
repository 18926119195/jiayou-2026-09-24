# call-0214-response.json

> **路径**: `snapshots\call-0214-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:15:49.378Z  

## 文件开头预览

```json
{
  "callId": "call-0214",
  "timestamp": "2026-09-24T10-15-48-677Z",
  "elapsed": 697,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【337】】",
    "usage": {
      "prompt_tokens": 3664,
      "completion_tokens": 5,
      "total_tokens": 3669,
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
    "id": "78f67840-15ce-4670-ad21-10fb9fa39915",
    "object": "chat.completion",
    "created": 1790244948,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【337】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3664,
      "completion_tokens": 5,
      "total_tokens": 3669,
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
