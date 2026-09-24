# call-0366-response.json

> **路径**: `snapshots\call-0366-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:16:35.087Z  

## 文件开头预览

```json
{
  "callId": "call-0366",
  "timestamp": "2026-09-24T10-16-34-083Z",
  "elapsed": 1001,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【122】】【【141】】【【146】】【【210】】【【213】】【【226】】【【307】】【【327】】",
    "usage": {
      "prompt_tokens": 3962,
      "completion_tokens": 33,
      "total_tokens": 3995,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3962
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "ad38f8f0-cde8-4eff-9605-5585a86f1f68",
    "object": "chat.completion",
    "created": 1790244994,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【122】】【【141】】【【146】】【【210】】【【213】】【【226】】【【307】】【【327】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3962,
      "completion_tokens": 33,
      "total_tokens": 3995,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3962
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
