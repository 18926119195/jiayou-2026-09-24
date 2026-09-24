# call-0060-response.json

> **路径**: `snapshots\call-0060-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:58:35.523Z  

## 文件开头预览

```json
{
  "callId": "call-0060",
  "timestamp": "2026-09-24T10-58-35-181Z",
  "elapsed": 341,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【256】】【【270】】【【305】】",
    "usage": {
      "prompt_tokens": 3684,
      "completion_tokens": 13,
      "total_tokens": 3697,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3684
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "28c33d87-5c1b-4a70-a7b1-9101edcf34b1",
    "object": "chat.completion",
    "created": 1790247515,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【256】】【【270】】【【305】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3684,
      "completion_tokens": 13,
      "total_tokens": 3697,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3684
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
