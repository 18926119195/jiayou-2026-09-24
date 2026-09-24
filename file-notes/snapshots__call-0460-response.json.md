# call-0460-response.json

> **路径**: `snapshots\call-0460-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:01.485Z  

## 文件开头预览

```json
{
  "callId": "call-0460",
  "timestamp": "2026-09-24T10-17-01-056Z",
  "elapsed": 426,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3378,
      "completion_tokens": 2,
      "total_tokens": 3380,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3378
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "6ab43120-49f2-4e23-be66-b5e8589f5d98",
    "object": "chat.completion",
    "created": 1790245021,
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
      "prompt_tokens": 3378,
      "completion_tokens": 2,
      "total_tokens": 3380,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3378
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
