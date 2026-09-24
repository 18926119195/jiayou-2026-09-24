# call-0627-response.json

> **路径**: `snapshots\call-0627-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:48.518Z  

## 文件开头预览

```json
{
  "callId": "call-0627",
  "timestamp": "2026-09-24T10-17-47-939Z",
  "elapsed": 575,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3170,
      "completion_tokens": 2,
      "total_tokens": 3172,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3170
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "23e48a71-fe78-46e7-a9cd-352b0065ac72",
    "object": "chat.completion",
    "created": 1790245068,
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
      "prompt_tokens": 3170,
      "completion_tokens": 2,
      "total_tokens": 3172,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3170
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
