# call-0300-response.json

> **路径**: `snapshots\call-0300-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:16:12.669Z  

## 文件开头预览

```json
{
  "callId": "call-0300",
  "timestamp": "2026-09-24T10-16-11-678Z",
  "elapsed": 989,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【3】】【【5】】【【296】】【【323】】【【329】】",
    "usage": {
      "prompt_tokens": 3502,
      "completion_tokens": 21,
      "total_tokens": 3523,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3502
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "c639289f-28dc-4a09-9e5a-31b8c2fa12a2",
    "object": "chat.completion",
    "created": 1790244971,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【3】】【【5】】【【296】】【【323】】【【329】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3502,
      "completion_tokens": 21,
      "total_tokens": 3523,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3502
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
