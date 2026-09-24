# call-0232-response.json

> **路径**: `snapshots\call-0232-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:15:58.028Z  

## 文件开头预览

```json
{
  "callId": "call-0232",
  "timestamp": "2026-09-24T10-15-57-422Z",
  "elapsed": 604,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【294】】【【335】】",
    "usage": {
      "prompt_tokens": 3781,
      "completion_tokens": 9,
      "total_tokens": 3790,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3781
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "823b2ddf-7184-4e5c-80e7-037fad4397d0",
    "object": "chat.completion",
    "created": 1790244957,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【294】】【【335】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3781,
      "completion_tokens": 9,
      "total_tokens": 3790,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3781
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
