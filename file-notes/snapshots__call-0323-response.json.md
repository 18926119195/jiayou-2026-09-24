# call-0323-response.json

> **路径**: `snapshots\call-0323-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:16:23.902Z  

## 文件开头预览

```json
{
  "callId": "call-0323",
  "timestamp": "2026-09-24T10-16-23-159Z",
  "elapsed": 742,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【8】】【【138】】【【150】】【【159】】【【215】】【【224】】【【290】】【【300】】",
    "usage": {
      "prompt_tokens": 3379,
      "completion_tokens": 33,
      "total_tokens": 3412,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3379
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "6c281fa4-fd71-43e8-b7e2-375e9ea42cc0",
    "object": "chat.completion",
    "created": 1790244983,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【8】】【【138】】【【150】】【【159】】【【215】】【【224】】【【290】】【【300】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3379,
      "completion_tokens": 33,
      "total_tokens": 3412,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3379
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
