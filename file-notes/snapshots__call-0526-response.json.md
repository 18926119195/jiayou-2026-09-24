# call-0526-response.json

> **路径**: `snapshots\call-0526-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:17:13.769Z  

## 文件开头预览

```json
{
  "callId": "call-0526",
  "timestamp": "2026-09-24T10-17-13-061Z",
  "elapsed": 706,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【191】】【【197】】【【244】】【【267】】【【320】】【【344】】【【345】】",
    "usage": {
      "prompt_tokens": 3672,
      "completion_tokens": 29,
      "total_tokens": 3701,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3672
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "0c7490e2-c25d-4f8f-bc51-392b9bae933b",
    "object": "chat.completion",
    "created": 1790245033,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【191】】【【197】】【【244】】【【267】】【【320】】【【344】】【【345】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3672,
      "completion_tokens": 29,
      "total_tokens": 3701,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3672
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
