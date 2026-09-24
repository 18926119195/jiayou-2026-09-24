# call-0467-response.json

> **路径**: `snapshots\call-0467-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:02.420Z  

## 文件开头预览

```json
{
  "callId": "call-0467",
  "timestamp": "2026-09-24T10-17-01-482Z",
  "elapsed": 934,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3793,
      "completion_tokens": 2,
      "total_tokens": 3795,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3793
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "a2e0cf4c-bb5c-4032-a439-6d7bb32b7b34",
    "object": "chat.completion",
    "created": 1790245021,
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
      "prompt_tokens": 3793,
      "completion_tokens": 2,
      "total_tokens": 3795,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3793
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
