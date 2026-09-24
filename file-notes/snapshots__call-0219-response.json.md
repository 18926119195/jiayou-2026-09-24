# call-0219-response.json

> **路径**: `snapshots\call-0219-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.5 KB  
> **最后修改**: 2026-09-24T10:15:49.821Z  

## 文件开头预览

```json
{
  "callId": "call-0219",
  "timestamp": "2026-09-24T10-15-49-004Z",
  "elapsed": 815,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【3】】【【4】】【【5】】【【7】】【【19】】【【20】】【【24】】【【25】】【【26】】【【27】】【【30】】【【44】】【【67】】【【211】】",
    "usage": {
      "prompt_tokens": 3107,
      "completion_tokens": 57,
      "total_tokens": 3164,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3107
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "742e644f-219b-477c-8ada-dfa116f31e98",
    "object": "chat.completion",
    "created": 1790244949,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【3】】【【4】】【【5】】【【7】】【【19】】【【20】】【【24】】【【25】】【【26】】【【27】】【【30】】【【44】】【【67】】【【211】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3107,
      "completion_tokens": 57,
      "total_tokens": 3164,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3107
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
