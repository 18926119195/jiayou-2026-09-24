# call-0574-response.json

> **路径**: `snapshots\call-0574-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:17:37.384Z  

## 文件开头预览

```json
{
  "callId": "call-0574",
  "timestamp": "2026-09-24T10-17-36-721Z",
  "elapsed": 661,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【65】】【【199】】【【287】】",
    "usage": {
      "prompt_tokens": 3862,
      "completion_tokens": 13,
      "total_tokens": 3875,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3862
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "176f8987-ed50-4bb9-be02-1d6ce59277c0",
    "object": "chat.completion",
    "created": 1790245056,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【65】】【【199】】【【287】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3862,
      "completion_tokens": 13,
      "total_tokens": 3875,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3862
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
