# call-0192-response.json

> **路径**: `snapshots\call-0192-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:15:46.984Z  

## 文件开头预览

```json
{
  "callId": "call-0192",
  "timestamp": "2026-09-24T10-15-46-614Z",
  "elapsed": 367,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【37】】【【263】】【【264】】【【289】】【【306】】",
    "usage": {
      "prompt_tokens": 3458,
      "completion_tokens": 21,
      "total_tokens": 3479,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3458
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "12f2ee7f-a42c-4c78-a633-e351c2cd545f",
    "object": "chat.completion",
    "created": 1790244946,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【37】】【【263】】【【264】】【【289】】【【306】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3458,
      "completion_tokens": 21,
      "total_tokens": 3479,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3458
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
