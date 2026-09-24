# call-0376-response.json

> **路径**: `snapshots\call-0376-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:16:35.820Z  

## 文件开头预览

```json
{
  "callId": "call-0376",
  "timestamp": "2026-09-24T10-16-35-122Z",
  "elapsed": 695,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【28】】【【93】】【【206】】【【253】】【【267】】",
    "usage": {
      "prompt_tokens": 3808,
      "completion_tokens": 21,
      "total_tokens": 3829,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3808
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "57a6b8eb-6198-43db-be62-fc144e78308b",
    "object": "chat.completion",
    "created": 1790244995,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【28】】【【93】】【【206】】【【253】】【【267】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3808,
      "completion_tokens": 21,
      "total_tokens": 3829,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3808
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
