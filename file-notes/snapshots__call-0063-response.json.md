# call-0063-response.json

> **路径**: `snapshots\call-0063-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:58:36.297Z  

## 文件开头预览

```json
{
  "callId": "call-0063",
  "timestamp": "2026-09-24T10-58-35-522Z",
  "elapsed": 774,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3631,
      "completion_tokens": 2,
      "total_tokens": 3633,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3631
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "c6ee5645-a2db-461c-a0b0-331624016832",
    "object": "chat.completion",
    "created": 1790247515,
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
      "prompt_tokens": 3631,
      "completion_tokens": 2,
      "total_tokens": 3633,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3631
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
