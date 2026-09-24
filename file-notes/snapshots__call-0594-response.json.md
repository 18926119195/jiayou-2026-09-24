# call-0594-response.json

> **路径**: `snapshots\call-0594-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:17:45.867Z  

## 文件开头预览

```json
{
  "callId": "call-0594",
  "timestamp": "2026-09-24T10-17-45-153Z",
  "elapsed": 711,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【3】】【【17】】【【28】】【【275】】【【317】】【【344】】",
    "usage": {
      "prompt_tokens": 3787,
      "completion_tokens": 25,
      "total_tokens": 3812,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3787
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "7470fb84-fded-49fc-8622-3f9eb5d751af",
    "object": "chat.completion",
    "created": 1790245065,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【3】】【【17】】【【28】】【【275】】【【317】】【【344】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3787,
      "completion_tokens": 25,
      "total_tokens": 3812,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3787
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
