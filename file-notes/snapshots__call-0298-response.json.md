# call-0298-response.json

> **路径**: `snapshots\call-0298-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:16:12.188Z  

## 文件开头预览

```json
{
  "callId": "call-0298",
  "timestamp": "2026-09-24T10-16-11-477Z",
  "elapsed": 708,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【50】】【【55】】【【59】】【【184】】【【201】】【【223】】",
    "usage": {
      "prompt_tokens": 3743,
      "completion_tokens": 25,
      "total_tokens": 3768,
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
    "id": "bb6c92a1-7c8f-438c-a1c2-6f4857a0c2eb",
    "object": "chat.completion",
    "created": 1790244971,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【50】】【【55】】【【59】】【【184】】【【201】】【【223】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3743,
      "completion_tokens": 25,
      "total_tokens": 3768,
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
