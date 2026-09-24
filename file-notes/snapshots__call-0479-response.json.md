# call-0479-response.json

> **路径**: `snapshots\call-0479-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:03.131Z  

## 文件开头预览

```json
{
  "callId": "call-0479",
  "timestamp": "2026-09-24T10-17-02-780Z",
  "elapsed": 347,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3850,
      "completion_tokens": 2,
      "total_tokens": 3852,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3850
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "713fd874-91c8-4b18-abdd-9a8e24b0fe60",
    "object": "chat.completion",
    "created": 1790245022,
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
      "prompt_tokens": 3850,
      "completion_tokens": 2,
      "total_tokens": 3852,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3850
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
