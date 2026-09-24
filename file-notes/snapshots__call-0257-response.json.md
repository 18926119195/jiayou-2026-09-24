# call-0257-response.json

> **路径**: `snapshots\call-0257-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:16:00.527Z  

## 文件开头预览

```json
{
  "callId": "call-0257",
  "timestamp": "2026-09-24T10-15-59-722Z",
  "elapsed": 803,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【199】】",
    "usage": {
      "prompt_tokens": 3860,
      "completion_tokens": 5,
      "total_tokens": 3865,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3860
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "f447d538-3f95-4faf-9501-72aa68272b34",
    "object": "chat.completion",
    "created": 1790244959,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【199】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3860,
      "completion_tokens": 5,
      "total_tokens": 3865,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3860
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
