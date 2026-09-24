# call-0116-response.json

> **路径**: `snapshots\call-0116-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:58:48.107Z  

## 文件开头预览

```json
{
  "callId": "call-0116",
  "timestamp": "2026-09-24T10-58-47-637Z",
  "elapsed": 468,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3622,
      "completion_tokens": 2,
      "total_tokens": 3624,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3622
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "029fa51d-7dbd-41f6-92e9-54c5cce14118",
    "object": "chat.completion",
    "created": 1790247527,
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
      "prompt_tokens": 3622,
      "completion_tokens": 2,
      "total_tokens": 3624,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3622
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
