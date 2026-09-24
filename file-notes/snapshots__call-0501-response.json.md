# call-0501-response.json

> **路径**: `snapshots\call-0501-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:17:10.976Z  

## 文件开头预览

```json
{
  "callId": "call-0501",
  "timestamp": "2026-09-24T10-17-10-394Z",
  "elapsed": 582,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【8】】【【97】】【【45】】【【40】】【【285】】【【339】】",
    "usage": {
      "prompt_tokens": 3784,
      "completion_tokens": 25,
      "total_tokens": 3809,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3784
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "74145b12-972d-4266-9473-9765b38a4b23",
    "object": "chat.completion",
    "created": 1790245030,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【8】】【【97】】【【45】】【【40】】【【285】】【【339】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3784,
      "completion_tokens": 25,
      "total_tokens": 3809,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3784
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
