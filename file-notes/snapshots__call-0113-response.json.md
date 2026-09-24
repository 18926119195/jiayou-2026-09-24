# call-0113-response.json

> **路径**: `snapshots\call-0113-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:58:47.638Z  

## 文件开头预览

```json
{
  "callId": "call-0113",
  "timestamp": "2026-09-24T10-58-47-251Z",
  "elapsed": 386,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【9】】【【42】】【【66】】【【225】】【【298】】",
    "usage": {
      "prompt_tokens": 3500,
      "completion_tokens": 21,
      "total_tokens": 3521,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3500
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "93f655da-5e36-471e-b6fc-a0781de5c9fd",
    "object": "chat.completion",
    "created": 1790247527,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【9】】【【42】】【【66】】【【225】】【【298】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3500,
      "completion_tokens": 21,
      "total_tokens": 3521,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3500
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
