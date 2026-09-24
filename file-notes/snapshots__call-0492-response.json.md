# call-0492-response.json

> **路径**: `snapshots\call-0492-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:04.475Z  

## 文件开头预览

```json
{
  "callId": "call-0492",
  "timestamp": "2026-09-24T10-17-03-951Z",
  "elapsed": 520,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【76】】",
    "usage": {
      "prompt_tokens": 3163,
      "completion_tokens": 5,
      "total_tokens": 3168,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3163
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "7a60f48e-ddd4-4644-81e4-3258bd0074b7",
    "object": "chat.completion",
    "created": 1790245024,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【76】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3163,
      "completion_tokens": 5,
      "total_tokens": 3168,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3163
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
