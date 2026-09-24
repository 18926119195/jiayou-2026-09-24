# call-0129-response.json

> **路径**: `snapshots\call-0129-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:58:49.848Z  

## 文件开头预览

```json
{
  "callId": "call-0129",
  "timestamp": "2026-09-24T10-58-49-324Z",
  "elapsed": 522,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【47】】【【92】】【【134】】【【138】】【【141】】【【297】】",
    "usage": {
      "prompt_tokens": 3514,
      "completion_tokens": 25,
      "total_tokens": 3539,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3514
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "5ab8b68a-5238-442c-bcf9-cc81d396772c",
    "object": "chat.completion",
    "created": 1790247529,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【47】】【【92】】【【134】】【【138】】【【141】】【【297】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3514,
      "completion_tokens": 25,
      "total_tokens": 3539,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3514
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
