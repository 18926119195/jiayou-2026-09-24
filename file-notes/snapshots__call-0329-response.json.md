# call-0329-response.json

> **路径**: `snapshots\call-0329-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:16:24.422Z  

## 文件开头预览

```json
{
  "callId": "call-0329",
  "timestamp": "2026-09-24T10-16-23-901Z",
  "elapsed": 519,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【28】】【【100】】【【167】】【【319】】【【354】】",
    "usage": {
      "prompt_tokens": 3801,
      "completion_tokens": 21,
      "total_tokens": 3822,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3801
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "de9f35d2-b4df-4aff-85b5-22bccf9f96fc",
    "object": "chat.completion",
    "created": 1790244984,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【28】】【【100】】【【167】】【【319】】【【354】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3801,
      "completion_tokens": 21,
      "total_tokens": 3822,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3801
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
