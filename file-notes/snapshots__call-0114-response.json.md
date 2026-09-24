# call-0114-response.json

> **路径**: `snapshots\call-0114-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:58:48.253Z  

## 文件开头预览

```json
{
  "callId": "call-0114",
  "timestamp": "2026-09-24T10-58-47-568Z",
  "elapsed": 682,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【102】】【【215】】【【300】】【【321】】",
    "usage": {
      "prompt_tokens": 3482,
      "completion_tokens": 17,
      "total_tokens": 3499,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3482
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "5f116e71-8851-4eef-bf4d-642cd1c385cc",
    "object": "chat.completion",
    "created": 1790247527,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【102】】【【215】】【【300】】【【321】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3482,
      "completion_tokens": 17,
      "total_tokens": 3499,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3482
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
