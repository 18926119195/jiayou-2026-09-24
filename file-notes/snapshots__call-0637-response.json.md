# call-0637-response.json

> **路径**: `snapshots\call-0637-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:57.280Z  

## 文件开头预览

```json
{
  "callId": "call-0637",
  "timestamp": "2026-09-24T10-17-56-548Z",
  "elapsed": 728,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3789,
      "completion_tokens": 2,
      "total_tokens": 3791,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3789
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "75a746c1-1c23-49e2-8647-22719b96a2a5",
    "object": "chat.completion",
    "created": 1790245076,
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
      "prompt_tokens": 3789,
      "completion_tokens": 2,
      "total_tokens": 3791,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3789
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
