# call-0592-response.json

> **路径**: `snapshots\call-0592-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:45.334Z  

## 文件开头预览

```json
{
  "callId": "call-0592",
  "timestamp": "2026-09-24T10-17-44-595Z",
  "elapsed": 736,
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
    "id": "884ad226-35f0-46ac-b647-97da512f4588",
    "object": "chat.completion",
    "created": 1790245064,
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
