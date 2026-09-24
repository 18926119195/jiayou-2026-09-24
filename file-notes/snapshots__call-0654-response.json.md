# call-0654-response.json

> **路径**: `snapshots\call-0654-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:17:58.484Z  

## 文件开头预览

```json
{
  "callId": "call-0654",
  "timestamp": "2026-09-24T10-17-58-012Z",
  "elapsed": 468,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【231】】",
    "usage": {
      "prompt_tokens": 3487,
      "completion_tokens": 5,
      "total_tokens": 3492,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3487
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "ca2eaa91-a2d7-4219-821e-d2979d05fdd4",
    "object": "chat.completion",
    "created": 1790245078,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【231】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3487,
      "completion_tokens": 5,
      "total_tokens": 3492,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3487
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
