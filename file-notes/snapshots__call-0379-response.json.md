# call-0379-response.json

> **路径**: `snapshots\call-0379-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:16:35.961Z  

## 文件开头预览

```json
{
  "callId": "call-0379",
  "timestamp": "2026-09-24T10-16-35-463Z",
  "elapsed": 496,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【324】】【【325】】",
    "usage": {
      "prompt_tokens": 3964,
      "completion_tokens": 9,
      "total_tokens": 3973,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3964
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "45b3e767-e4ea-461e-b5ad-066276f3006f",
    "object": "chat.completion",
    "created": 1790244995,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【324】】【【325】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3964,
      "completion_tokens": 9,
      "total_tokens": 3973,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3964
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
