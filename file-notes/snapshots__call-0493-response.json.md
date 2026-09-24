# call-0493-response.json

> **路径**: `snapshots\call-0493-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:04.397Z  

## 文件开头预览

```json
{
  "callId": "call-0493",
  "timestamp": "2026-09-24T10-17-04-007Z",
  "elapsed": 387,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 1680,
      "completion_tokens": 2,
      "total_tokens": 1682,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 1680
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "898d02f3-c846-4e94-9e71-671b7d431576",
    "object": "chat.completion",
    "created": 1790245024,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "NONE"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 1680,
      "completion_tokens": 2,
      "total_tokens": 1682,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 1680
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
