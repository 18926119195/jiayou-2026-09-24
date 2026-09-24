# call-0656-response.json

> **路径**: `snapshots\call-0656-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:58.575Z  

## 文件开头预览

```json
{
  "callId": "call-0656",
  "timestamp": "2026-09-24T10-17-58-199Z",
  "elapsed": 372,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【8】】",
    "usage": {
      "prompt_tokens": 3282,
      "completion_tokens": 5,
      "total_tokens": 3287,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3282
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "ab96204c-db45-421f-9176-27325e466565",
    "object": "chat.completion",
    "created": 1790245078,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【8】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3282,
      "completion_tokens": 5,
      "total_tokens": 3287,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3282
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
