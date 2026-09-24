# call-0290-response.json

> **路径**: `snapshots\call-0290-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:16:11.378Z  

## 文件开头预览

```json
{
  "callId": "call-0290",
  "timestamp": "2026-09-24T10-16-10-494Z",
  "elapsed": 881,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【45】】【【83】】【【137】】【【138】】【【287】】【【294】】【【296】】",
    "usage": {
      "prompt_tokens": 3488,
      "completion_tokens": 29,
      "total_tokens": 3517,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3488
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "ee8aa0e1-b46b-4227-9daa-baeb2c601720",
    "object": "chat.completion",
    "created": 1790244970,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【45】】【【83】】【【137】】【【138】】【【287】】【【294】】【【296】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3488,
      "completion_tokens": 29,
      "total_tokens": 3517,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3488
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
