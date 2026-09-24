# call-0284-response.json

> **路径**: `snapshots\call-0284-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:16:10.396Z  

## 文件开头预览

```json
{
  "callId": "call-0284",
  "timestamp": "2026-09-24T10-16-10-042Z",
  "elapsed": 353,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3801,
      "completion_tokens": 2,
      "total_tokens": 3803,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3801
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "bdf3a5a4-17da-42a4-8dc1-5bac8578b175",
    "object": "chat.completion",
    "created": 1790244970,
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
      "prompt_tokens": 3801,
      "completion_tokens": 2,
      "total_tokens": 3803,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3801
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
