# call-0617-response.json

> **路径**: `snapshots\call-0617-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:17:48.071Z  

## 文件开头预览

```json
{
  "callId": "call-0617",
  "timestamp": "2026-09-24T10-17-47-212Z",
  "elapsed": 855,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【141】】【【364】】【【365】】",
    "usage": {
      "prompt_tokens": 3681,
      "completion_tokens": 13,
      "total_tokens": 3694,
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
    "id": "c0f1101b-ef90-44b2-a969-bb2d4636b973",
    "object": "chat.completion",
    "created": 1790245067,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【141】】【【364】】【【365】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3681,
      "completion_tokens": 13,
      "total_tokens": 3694,
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
