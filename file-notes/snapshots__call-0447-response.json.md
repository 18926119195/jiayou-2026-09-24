# call-0447-response.json

> **路径**: `snapshots\call-0447-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:16:52.547Z  

## 文件开头预览

```json
{
  "callId": "call-0447",
  "timestamp": "2026-09-24T10-16-51-839Z",
  "elapsed": 705,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【21】】【【72】】【【167】】【【211】】",
    "usage": {
      "prompt_tokens": 3163,
      "completion_tokens": 17,
      "total_tokens": 3180,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3163
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "bd59213f-a23f-4d8b-aabe-4a91e30beb5b",
    "object": "chat.completion",
    "created": 1790245012,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【21】】【【72】】【【167】】【【211】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3163,
      "completion_tokens": 17,
      "total_tokens": 3180,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3163
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
