# call-0475-response.json

> **路径**: `snapshots\call-0475-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:17:02.952Z  

## 文件开头预览

```json
{
  "callId": "call-0475",
  "timestamp": "2026-09-24T10-17-02-417Z",
  "elapsed": 531,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【37】】【【221】】【【223】】【【252】】【【253】】【【287】】",
    "usage": {
      "prompt_tokens": 3681,
      "completion_tokens": 25,
      "total_tokens": 3706,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3681
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "a2d8ac14-71d5-4069-add0-9486303657c3",
    "object": "chat.completion",
    "created": 1790245022,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【37】】【【221】】【【223】】【【252】】【【253】】【【287】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3681,
      "completion_tokens": 25,
      "total_tokens": 3706,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3681
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
