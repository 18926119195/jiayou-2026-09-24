# call-0307-response.json

> **路径**: `snapshots\call-0307-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:16:13.000Z  

## 文件开头预览

```json
{
  "callId": "call-0307",
  "timestamp": "2026-09-24T10-16-12-402Z",
  "elapsed": 596,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【42】】【【63】】【【209】】【【210】】【【241】】【【273】】【【274】】",
    "usage": {
      "prompt_tokens": 3278,
      "completion_tokens": 29,
      "total_tokens": 3307,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3278
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "10c5442b-bd04-4afd-85ae-751ceb2c2f78",
    "object": "chat.completion",
    "created": 1790244972,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【42】】【【63】】【【209】】【【210】】【【241】】【【273】】【【274】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3278,
      "completion_tokens": 29,
      "total_tokens": 3307,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3278
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
