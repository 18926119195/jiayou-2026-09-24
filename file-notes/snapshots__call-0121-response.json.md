# call-0121-response.json

> **路径**: `snapshots\call-0121-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:58:48.779Z  

## 文件开头预览

```json
{
  "callId": "call-0121",
  "timestamp": "2026-09-24T10-58-48-251Z",
  "elapsed": 525,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【21】】【【198】】【【255】】【【341】】【【346】】",
    "usage": {
      "prompt_tokens": 3836,
      "completion_tokens": 21,
      "total_tokens": 3857,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3836
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "e5ae0f6b-8483-49ae-9d0a-258c9ffde138",
    "object": "chat.completion",
    "created": 1790247528,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【21】】【【198】】【【255】】【【341】】【【346】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3836,
      "completion_tokens": 21,
      "total_tokens": 3857,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3836
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
