# call-0252-response.json

> **路径**: `snapshots\call-0252-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:15:59.824Z  

## 文件开头预览

```json
{
  "callId": "call-0252",
  "timestamp": "2026-09-24T10-15-59-321Z",
  "elapsed": 500,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【143】】【【279】】【【377】】",
    "usage": {
      "prompt_tokens": 3851,
      "completion_tokens": 13,
      "total_tokens": 3864,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3851
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "927fbec9-0eff-4d5f-af9d-e864ba877b39",
    "object": "chat.completion",
    "created": 1790244959,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【143】】【【279】】【【377】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3851,
      "completion_tokens": 13,
      "total_tokens": 3864,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3851
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
