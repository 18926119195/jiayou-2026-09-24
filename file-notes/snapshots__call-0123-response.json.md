# call-0123-response.json

> **路径**: `snapshots\call-0123-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.5 KB  
> **最后修改**: 2026-09-24T10:58:49.437Z  

## 文件开头预览

```json
{
  "callId": "call-0123",
  "timestamp": "2026-09-24T10-58-48-580Z",
  "elapsed": 855,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【5】】【【18】】【【19】】【【47】】【【64】】【【65】】【【69】】【【70】】【【185】】【【189】】【【190】】【【191】】【【323】】【【331】】【【357】】",
    "usage": {
      "prompt_tokens": 3664,
      "completion_tokens": 61,
      "total_tokens": 3725,
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
    "id": "0cd7493f-1b70-4e86-9639-39da4857f338",
    "object": "chat.completion",
    "created": 1790247528,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【5】】【【18】】【【19】】【【47】】【【64】】【【65】】【【69】】【【70】】【【185】】【【189】】【【190】】【【191】】【【323】】【【331】】【【357】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3664,
      "completion_tokens": 61,
      "total_tokens": 3725,
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
