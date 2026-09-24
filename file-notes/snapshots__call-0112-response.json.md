# call-0112-response.json

> **路径**: `snapshots\call-0112-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:58:47.962Z  

## 文件开头预览

```json
{
  "callId": "call-0112",
  "timestamp": "2026-09-24T10-58-47-206Z",
  "elapsed": 753,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【10】】【【18】】【【43】】【【81】】【【99】】【【295】】",
    "usage": {
      "prompt_tokens": 3771,
      "completion_tokens": 25,
      "total_tokens": 3796,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3771
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "9b658c2a-ea10-4bfe-b493-e5a72625ee0b",
    "object": "chat.completion",
    "created": 1790247527,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【10】】【【18】】【【43】】【【81】】【【99】】【【295】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3771,
      "completion_tokens": 25,
      "total_tokens": 3796,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3771
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
