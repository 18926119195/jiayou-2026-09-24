# call-0195-response.json

> **路径**: `snapshots\call-0195-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:15:47.482Z  

## 文件开头预览

```json
{
  "callId": "call-0195",
  "timestamp": "2026-09-24T10-15-46-888Z",
  "elapsed": 592,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3796,
      "completion_tokens": 2,
      "total_tokens": 3798,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3796
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "93e0d72e-4404-4186-b057-015840dbf4df",
    "object": "chat.completion",
    "created": 1790244947,
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
      "prompt_tokens": 3796,
      "completion_tokens": 2,
      "total_tokens": 3798,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3796
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
