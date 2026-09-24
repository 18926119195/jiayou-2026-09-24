# call-0212-response.json

> **路径**: `snapshots\call-0212-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:15:49.006Z  

## 文件开头预览

```json
{
  "callId": "call-0212",
  "timestamp": "2026-09-24T10-15-48-368Z",
  "elapsed": 635,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3862,
      "completion_tokens": 2,
      "total_tokens": 3864,
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
    "id": "ac183339-71dc-4371-9a40-f3f91f182ec1",
    "object": "chat.completion",
    "created": 1790244948,
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
      "prompt_tokens": 3862,
      "completion_tokens": 2,
      "total_tokens": 3864,
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
