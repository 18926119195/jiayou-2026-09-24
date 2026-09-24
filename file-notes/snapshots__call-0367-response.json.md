# call-0367-response.json

> **路径**: `snapshots\call-0367-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:16:35.124Z  

## 文件开头预览

```json
{
  "callId": "call-0367",
  "timestamp": "2026-09-24T10-16-34-084Z",
  "elapsed": 1038,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【51】】【【106】】【【118】】",
    "usage": {
      "prompt_tokens": 3794,
      "completion_tokens": 13,
      "total_tokens": 3807,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3794
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "ace5fd15-2965-47e7-9197-a5e3f7ba1750",
    "object": "chat.completion",
    "created": 1790244994,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【51】】【【106】】【【118】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3794,
      "completion_tokens": 13,
      "total_tokens": 3807,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3794
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
