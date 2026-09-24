# call-0437-response.json

> **路径**: `snapshots\call-0437-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:16:51.784Z  

## 文件开头预览

```json
{
  "callId": "call-0437",
  "timestamp": "2026-09-24T10-16-51-187Z",
  "elapsed": 594,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【363】】【【364】】【【365】】【【366】】",
    "usage": {
      "prompt_tokens": 3674,
      "completion_tokens": 17,
      "total_tokens": 3691,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3674
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "d370e50f-d28f-434d-8654-33968b388dcf",
    "object": "chat.completion",
    "created": 1790245011,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【363】】【【364】】【【365】】【【366】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3674,
      "completion_tokens": 17,
      "total_tokens": 3691,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3674
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
