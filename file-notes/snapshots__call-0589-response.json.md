# call-0589-response.json

> **路径**: `snapshots\call-0589-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:17:45.448Z  

## 文件开头预览

```json
{
  "callId": "call-0589",
  "timestamp": "2026-09-24T10-17-44-593Z",
  "elapsed": 852,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【7】】【【117】】【【269】】【【389】】【【398】】【【399】】【【415】】",
    "usage": {
      "prompt_tokens": 4086,
      "completion_tokens": 29,
      "total_tokens": 4115,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 4086
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "d09b3d9d-b0bd-42c5-b3df-6bc9adf3e5fe",
    "object": "chat.completion",
    "created": 1790245065,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【7】】【【117】】【【269】】【【389】】【【398】】【【399】】【【415】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 4086,
      "completion_tokens": 29,
      "total_tokens": 4115,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 4086
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
