# call-0025-response.json

> **路径**: `snapshots\call-0025-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T12:14:12.714Z  

## 文件开头预览

```json
{
  "callId": "call-0025",
  "timestamp": "2026-09-24T12-14-12-102Z",
  "elapsed": 610,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3615,
      "completion_tokens": 2,
      "total_tokens": 3617,
      "prompt_tokens_details": {
        "cached_tokens": 3456
      },
      "prompt_cache_hit_tokens": 3456,
      "prompt_cache_miss_tokens": 159
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "44b9f414-9e23-4745-9c61-8a45ee28c667",
    "object": "chat.completion",
    "created": 1790252052,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "NONE"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3615,
      "completion_tokens": 2,
      "total_tokens": 3617,
      "prompt_tokens_details": {
        "cached_tokens": 3456
      },
      "prompt_cache_hit_tokens": 3456,
      "prompt_cache_miss_tokens": 159
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
