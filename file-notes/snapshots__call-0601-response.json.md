# call-0601-response.json

> **路径**: `snapshots\call-0601-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:46.177Z  

## 文件开头预览

```json
{
  "callId": "call-0601",
  "timestamp": "2026-09-24T10-17-45-865Z",
  "elapsed": 310,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3807,
      "completion_tokens": 2,
      "total_tokens": 3809,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3807
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "a901dbaf-3f70-4308-9b14-4af428949ae6",
    "object": "chat.completion",
    "created": 1790245066,
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
      "prompt_tokens": 3807,
      "completion_tokens": 2,
      "total_tokens": 3809,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3807
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
