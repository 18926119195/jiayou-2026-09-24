# call-0120-response.json

> **路径**: `snapshots\call-0120-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.6 KB  
> **最后修改**: 2026-09-24T10:58:48.785Z  

## 文件开头预览

```json
{
  "callId": "call-0120",
  "timestamp": "2026-09-24T10-58-48-106Z",
  "elapsed": 676,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【115】】【【118】】【【135】】【【205】】【【236】】【【237】】【【238】】【【304】】【【305】】【【322】】【【337】】【【348】】【【349】】【【359】】【【360】】【【362】】",
    "usage": {
      "prompt_tokens": 3721,
      "completion_tokens": 65,
      "total_tokens": 3786,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3721
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "2b3c65d5-be1e-4763-8fc0-3088b6e19ec5",
    "object": "chat.completion",
    "created": 1790247528,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【115】】【【118】】【【135】】【【205】】【【236】】【【237】】【【238】】【【304】】【【305】】【【322】】【【337】】【【348】】【【349】】【【359】】【【360】】【【362】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3721,
      "completion_tokens": 65,
      "total_tokens": 3786,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3721
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
