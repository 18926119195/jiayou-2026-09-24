# call-0109-response.json

> **路径**: `snapshots\call-0109-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:58:47.570Z  

## 文件开头预览

```json
{
  "callId": "call-0109",
  "timestamp": "2026-09-24T10-58-47-031Z",
  "elapsed": 536,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3599,
      "completion_tokens": 2,
      "total_tokens": 3601,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3599
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "c2ecad3f-d512-43e7-8202-c25254b3258f",
    "object": "chat.completion",
    "created": 1790247527,
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
      "prompt_tokens": 3599,
      "completion_tokens": 2,
      "total_tokens": 3601,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3599
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
