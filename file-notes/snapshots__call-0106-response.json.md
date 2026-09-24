# call-0106-response.json

> **路径**: `snapshots\call-0106-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:58:47.182Z  

## 文件开头预览

```json
{
  "callId": "call-0106",
  "timestamp": "2026-09-24T10-58-46-698Z",
  "elapsed": 481,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3593,
      "completion_tokens": 2,
      "total_tokens": 3595,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3593
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "c0dd1477-a95c-41df-a650-f36b561f5620",
    "object": "chat.completion",
    "created": 1790247526,
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
      "prompt_tokens": 3593,
      "completion_tokens": 2,
      "total_tokens": 3595,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3593
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
