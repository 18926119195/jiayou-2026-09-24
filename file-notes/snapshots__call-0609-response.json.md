# call-0609-response.json

> **路径**: `snapshots\call-0609-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:17:47.046Z  

## 文件开头预览

```json
{
  "callId": "call-0609",
  "timestamp": "2026-09-24T10-17-46-393Z",
  "elapsed": 649,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【231】】【【317】】【【320】】【【182】】【【34】】【【295】】",
    "usage": {
      "prompt_tokens": 3491,
      "completion_tokens": 25,
      "total_tokens": 3516,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3491
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "80f17047-ea86-42e0-9008-f0435424a65e",
    "object": "chat.completion",
    "created": 1790245066,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【231】】【【317】】【【320】】【【182】】【【34】】【【295】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3491,
      "completion_tokens": 25,
      "total_tokens": 3516,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3491
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
