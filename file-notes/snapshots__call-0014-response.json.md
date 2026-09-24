# call-0014-response.json

> **路径**: `snapshots\call-0014-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T12:14:11.945Z  

## 文件开头预览

```json
{
  "callId": "call-0014",
  "timestamp": "2026-09-24T12-14-11-283Z",
  "elapsed": 661,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【256】】【【270】】【【305】】",
    "usage": {
      "prompt_tokens": 3684,
      "completion_tokens": 13,
      "total_tokens": 3697,
      "prompt_tokens_details": {
        "cached_tokens": 3456
      },
      "prompt_cache_hit_tokens": 3456,
      "prompt_cache_miss_tokens": 228
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "cf06b6c1-5052-41d9-bb41-8729b6e4f6f0",
    "object": "chat.completion",
    "created": 1790252051,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【256】】【【270】】【【305】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3684,
      "completion_tokens": 13,
      "total_tokens": 3697,
      "prompt_tokens_details": {
        "cached_tokens": 3456
      },
      "prompt_cache_hit_tokens": 3456,
      "prompt_cache_miss_tokens": 228
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
