# call-0552-response.json

> **路径**: `snapshots\call-0552-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:35.336Z  

## 文件开头预览

```json
{
  "callId": "call-0552",
  "timestamp": "2026-09-24T10-17-34-678Z",
  "elapsed": 654,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3738,
      "completion_tokens": 2,
      "total_tokens": 3740,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3738
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "e2dc05d7-e9dd-4d67-8646-ebc12e52f5ac",
    "object": "chat.completion",
    "created": 1790245054,
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
      "prompt_tokens": 3738,
      "completion_tokens": 2,
      "total_tokens": 3740,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3738
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
