# call-0256-response.json

> **路径**: `snapshots\call-0256-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:16:00.380Z  

## 文件开头预览

```json
{
  "callId": "call-0256",
  "timestamp": "2026-09-24T10-15-59-689Z",
  "elapsed": 687,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【3】】",
    "usage": {
      "prompt_tokens": 3495,
      "completion_tokens": 5,
      "total_tokens": 3500,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3495
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "71853fe3-93d7-40f9-b9ad-04ead2ff65ce",
    "object": "chat.completion",
    "created": 1790244959,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【3】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3495,
      "completion_tokens": 5,
      "total_tokens": 3500,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3495
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
