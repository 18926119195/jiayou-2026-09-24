# call-0657-response.json

> **路径**: `snapshots\call-0657-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:58.930Z  

## 文件开头预览

```json
{
  "callId": "call-0657",
  "timestamp": "2026-09-24T10-17-58-266Z",
  "elapsed": 660,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【14】】",
    "usage": {
      "prompt_tokens": 3256,
      "completion_tokens": 5,
      "total_tokens": 3261,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3256
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "8fd298f7-3a4e-47b0-8a89-c73769b40104",
    "object": "chat.completion",
    "created": 1790245078,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【14】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3256,
      "completion_tokens": 5,
      "total_tokens": 3261,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3256
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
