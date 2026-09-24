# call-0622-response.json

> **路径**: `snapshots\call-0622-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:48.054Z  

## 文件开头预览

```json
{
  "callId": "call-0622",
  "timestamp": "2026-09-24T10-17-47-521Z",
  "elapsed": 529,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3614,
      "completion_tokens": 2,
      "total_tokens": 3616,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3614
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "bdbac079-7068-4b51-b909-d124488e2c3c",
    "object": "chat.completion",
    "created": 1790245067,
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
      "prompt_tokens": 3614,
      "completion_tokens": 2,
      "total_tokens": 3616,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3614
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
