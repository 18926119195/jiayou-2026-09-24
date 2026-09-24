# call-0480-response.json

> **路径**: `snapshots\call-0480-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:17:03.620Z  

## 文件开头预览

```json
{
  "callId": "call-0480",
  "timestamp": "2026-09-24T10-17-02-821Z",
  "elapsed": 796,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【15】】【【50】】【【275】】",
    "usage": {
      "prompt_tokens": 3653,
      "completion_tokens": 13,
      "total_tokens": 3666,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3653
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "e2fbb7e9-26c2-4d34-a47e-b892236b4326",
    "object": "chat.completion",
    "created": 1790245023,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【15】】【【50】】【【275】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3653,
      "completion_tokens": 13,
      "total_tokens": 3666,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3653
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
