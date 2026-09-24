# call-0391-response.json

> **路径**: `snapshots\call-0391-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:16:36.969Z  

## 文件开头预览

```json
{
  "callId": "call-0391",
  "timestamp": "2026-09-24T10-16-36-537Z",
  "elapsed": 429,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【55】】【【348】】",
    "usage": {
      "prompt_tokens": 3743,
      "completion_tokens": 9,
      "total_tokens": 3752,
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
    "id": "d0965f5d-3c02-44e6-877f-33c2f7dcabff",
    "object": "chat.completion",
    "created": 1790244996,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【55】】【【348】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3743,
      "completion_tokens": 9,
      "total_tokens": 3752,
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
