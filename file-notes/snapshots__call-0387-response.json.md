# call-0387-response.json

> **路径**: `snapshots\call-0387-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:16:36.559Z  

## 文件开头预览

```json
{
  "callId": "call-0387",
  "timestamp": "2026-09-24T10-16-35-988Z",
  "elapsed": 569,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【163】】【【166】】【【243】】【【250】】【【263】】【【266】】【【286】】",
    "usage": {
      "prompt_tokens": 3261,
      "completion_tokens": 29,
      "total_tokens": 3290,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3261
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "a3dca1b9-8ef3-4d36-babd-c181fb39d835",
    "object": "chat.completion",
    "created": 1790244996,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【163】】【【166】】【【243】】【【250】】【【263】】【【266】】【【286】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3261,
      "completion_tokens": 29,
      "total_tokens": 3290,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3261
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
