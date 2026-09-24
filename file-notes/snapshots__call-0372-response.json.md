# call-0372-response.json

> **路径**: `snapshots\call-0372-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:16:35.577Z  

## 文件开头预览

```json
{
  "callId": "call-0372",
  "timestamp": "2026-09-24T10-16-34-797Z",
  "elapsed": 778,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【29】】【【30】】【【31】】【【33】】【【34】】【【35】】【【150】】【【364】】",
    "usage": {
      "prompt_tokens": 3743,
      "completion_tokens": 33,
      "total_tokens": 3776,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3743
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "dd9fdedf-2543-4c63-84e9-5cac4c4fd3bf",
    "object": "chat.completion",
    "created": 1790244995,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【29】】【【30】】【【31】】【【33】】【【34】】【【35】】【【150】】【【364】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3743,
      "completion_tokens": 33,
      "total_tokens": 3776,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3743
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
