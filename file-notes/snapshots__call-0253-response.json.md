# call-0253-response.json

> **路径**: `snapshots\call-0253-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:15:59.881Z  

## 文件开头预览

```json
{
  "callId": "call-0253",
  "timestamp": "2026-09-24T10-15-59-341Z",
  "elapsed": 537,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【15】】【【50】】",
    "usage": {
      "prompt_tokens": 3654,
      "completion_tokens": 9,
      "total_tokens": 3663,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3654
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "0a3074be-6b47-42bb-8ff4-48993d28c2b7",
    "object": "chat.completion",
    "created": 1790244959,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【15】】【【50】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3654,
      "completion_tokens": 9,
      "total_tokens": 3663,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3654
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
