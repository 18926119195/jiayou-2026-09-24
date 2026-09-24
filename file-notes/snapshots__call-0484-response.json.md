# call-0484-response.json

> **路径**: `snapshots\call-0484-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:04.030Z  

## 文件开头预览

```json
{
  "callId": "call-0484",
  "timestamp": "2026-09-24T10-17-03-316Z",
  "elapsed": 710,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3859,
      "completion_tokens": 2,
      "total_tokens": 3861,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3859
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "9f52d78c-bc2a-4507-b617-96e2b4211891",
    "object": "chat.completion",
    "created": 1790245023,
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
      "prompt_tokens": 3859,
      "completion_tokens": 2,
      "total_tokens": 3861,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3859
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
