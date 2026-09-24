# call-0436-response.json

> **路径**: `snapshots\call-0436-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:16:51.734Z  

## 文件开头预览

```json
{
  "callId": "call-0436",
  "timestamp": "2026-09-24T10-16-51-137Z",
  "elapsed": 595,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【1】】【【50】】【【55】】【【184】】【【285】】【【286】】【【348】】【【372】】",
    "usage": {
      "prompt_tokens": 3735,
      "completion_tokens": 33,
      "total_tokens": 3768,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3735
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "230e55f1-4dd1-413e-a7b1-b2fcdddfa3e6",
    "object": "chat.completion",
    "created": 1790245011,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【1】】【【50】】【【55】】【【184】】【【285】】【【286】】【【348】】【【372】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3735,
      "completion_tokens": 33,
      "total_tokens": 3768,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3735
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
