# call-0478-response.json

> **路径**: `snapshots\call-0478-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:17:03.466Z  

## 文件开头预览

```json
{
  "callId": "call-0478",
  "timestamp": "2026-09-24T10-17-02-765Z",
  "elapsed": 698,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【2】】【【5】】【【10】】【【28】】【【90】】【【106】】【【171】】【【191】】【【226】】【【227】】",
    "usage": {
      "prompt_tokens": 3531,
      "completion_tokens": 41,
      "total_tokens": 3572,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3531
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "c6c636fa-fcd6-48ed-a7ae-ffb610c1c214",
    "object": "chat.completion",
    "created": 1790245022,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【2】】【【5】】【【10】】【【28】】【【90】】【【106】】【【171】】【【191】】【【226】】【【227】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3531,
      "completion_tokens": 41,
      "total_tokens": 3572,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3531
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
