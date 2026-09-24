# call-0187-response.json

> **路径**: `snapshots\call-0187-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:15:46.889Z  

## 文件开头预览

```json
{
  "callId": "call-0187",
  "timestamp": "2026-09-24T10-15-46-405Z",
  "elapsed": 482,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【255】】【【256】】",
    "usage": {
      "prompt_tokens": 3783,
      "completion_tokens": 9,
      "total_tokens": 3792,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3783
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "0e540652-2916-4165-908d-8c6e0cb72f4b",
    "object": "chat.completion",
    "created": 1790244946,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【255】】【【256】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3783,
      "completion_tokens": 9,
      "total_tokens": 3792,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3783
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
