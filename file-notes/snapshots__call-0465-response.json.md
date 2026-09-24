# call-0465-response.json

> **路径**: `snapshots\call-0465-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:17:01.916Z  

## 文件开头预览

```json
{
  "callId": "call-0465",
  "timestamp": "2026-09-24T10-17-01-376Z",
  "elapsed": 536,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【86】】【【206】】【【207】】【【208】】【【209】】【【210】】",
    "usage": {
      "prompt_tokens": 3344,
      "completion_tokens": 25,
      "total_tokens": 3369,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3344
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "7706946a-278d-433a-92c5-450e99cc9770",
    "object": "chat.completion",
    "created": 1790245021,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【86】】【【206】】【【207】】【【208】】【【209】】【【210】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3344,
      "completion_tokens": 25,
      "total_tokens": 3369,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3344
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
