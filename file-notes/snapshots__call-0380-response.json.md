# call-0380-response.json

> **路径**: `snapshots\call-0380-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:16:36.014Z  

## 文件开头预览

```json
{
  "callId": "call-0380",
  "timestamp": "2026-09-24T10-16-35-514Z",
  "elapsed": 498,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【13】】【【14】】【【147】】【【175】】【【185】】【【311】】",
    "usage": {
      "prompt_tokens": 3993,
      "completion_tokens": 25,
      "total_tokens": 4018,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3993
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "34d101bb-9678-4417-afa9-8ca630a53938",
    "object": "chat.completion",
    "created": 1790244995,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【13】】【【14】】【【147】】【【175】】【【185】】【【311】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3993,
      "completion_tokens": 25,
      "total_tokens": 4018,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3993
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
