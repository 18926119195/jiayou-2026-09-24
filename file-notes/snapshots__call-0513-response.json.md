# call-0513-response.json

> **路径**: `snapshots\call-0513-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:17:12.330Z  

## 文件开头预览

```json
{
  "callId": "call-0513",
  "timestamp": "2026-09-24T10-17-11-945Z",
  "elapsed": 383,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【31】】【【295】】【【296】】【【343】】",
    "usage": {
      "prompt_tokens": 3954,
      "completion_tokens": 17,
      "total_tokens": 3971,
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
    "id": "8062f158-9aeb-42fd-8443-3a28a2b5fb1e",
    "object": "chat.completion",
    "created": 1790245032,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【31】】【【295】】【【296】】【【343】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3954,
      "completion_tokens": 17,
      "total_tokens": 3971,
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
