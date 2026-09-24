# call-0209-response.json

> **路径**: `snapshots\call-0209-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:15:48.816Z  

## 文件开头预览

```json
{
  "callId": "call-0209",
  "timestamp": "2026-09-24T10-15-48-205Z",
  "elapsed": 608,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【50】】【【55】】【【59】】【【184】】【【201】】【【285】】【【286】】",
    "usage": {
      "prompt_tokens": 3738,
      "completion_tokens": 29,
      "total_tokens": 3767,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3738
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "42cf2ed5-6876-4829-b467-c9d063196dd1",
    "object": "chat.completion",
    "created": 1790244948,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【50】】【【55】】【【59】】【【184】】【【201】】【【285】】【【286】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3738,
      "completion_tokens": 29,
      "total_tokens": 3767,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3738
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
