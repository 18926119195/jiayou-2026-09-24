# call-0568-response.json

> **路径**: `snapshots\call-0568-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:17:36.674Z  

## 文件开头预览

```json
{
  "callId": "call-0568",
  "timestamp": "2026-09-24T10-17-36-176Z",
  "elapsed": 495,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【1】】【【2】】【【78】】【【138】】【【253】】【【358】】",
    "usage": {
      "prompt_tokens": 3534,
      "completion_tokens": 25,
      "total_tokens": 3559,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3534
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "7c4466f2-a576-4438-bf2b-341c02e6b89a",
    "object": "chat.completion",
    "created": 1790245056,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【1】】【【2】】【【78】】【【138】】【【253】】【【358】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3534,
      "completion_tokens": 25,
      "total_tokens": 3559,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3534
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
