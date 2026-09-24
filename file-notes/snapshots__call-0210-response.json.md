# call-0210-response.json

> **路径**: `snapshots\call-0210-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:15:49.021Z  

## 文件开头预览

```json
{
  "callId": "call-0210",
  "timestamp": "2026-09-24T10-15-48-275Z",
  "elapsed": 744,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【102】】【【181】】【【269】】【【364】】【【365】】【【366】】",
    "usage": {
      "prompt_tokens": 3677,
      "completion_tokens": 25,
      "total_tokens": 3702,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3677
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "1484aa42-4bb7-48ea-8ddc-c484e551368f",
    "object": "chat.completion",
    "created": 1790244948,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【102】】【【181】】【【269】】【【364】】【【365】】【【366】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3677,
      "completion_tokens": 25,
      "total_tokens": 3702,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3677
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
