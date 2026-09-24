# call-0206-response.json

> **路径**: `snapshots\call-0206-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:15:48.552Z  

## 文件开头预览

```json
{
  "callId": "call-0206",
  "timestamp": "2026-09-24T10-15-48-020Z",
  "elapsed": 528,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【2】】【【28】】【【226】】【【227】】",
    "usage": {
      "prompt_tokens": 3534,
      "completion_tokens": 17,
      "total_tokens": 3551,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3534
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "a7295d0f-3aa7-407a-a7aa-36154cc7d367",
    "object": "chat.completion",
    "created": 1790244948,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【2】】【【28】】【【226】】【【227】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3534,
      "completion_tokens": 17,
      "total_tokens": 3551,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3534
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
