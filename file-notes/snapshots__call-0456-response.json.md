# call-0456-response.json

> **路径**: `snapshots\call-0456-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:17:01.057Z  

## 文件开头预览

```json
{
  "callId": "call-0456",
  "timestamp": "2026-09-24T10-17-00-401Z",
  "elapsed": 653,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【122】】【【223】】【【226】】【【312】】【【376】】",
    "usage": {
      "prompt_tokens": 3954,
      "completion_tokens": 21,
      "total_tokens": 3975,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3954
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "995e5c2b-3d7c-4940-b292-eee6125a0682",
    "object": "chat.completion",
    "created": 1790245020,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【122】】【【223】】【【226】】【【312】】【【376】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3954,
      "completion_tokens": 21,
      "total_tokens": 3975,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3954
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
