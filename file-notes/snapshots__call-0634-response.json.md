# call-0634-response.json

> **路径**: `snapshots\call-0634-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:57.053Z  

## 文件开头预览

```json
{
  "callId": "call-0634",
  "timestamp": "2026-09-24T10-17-56-546Z",
  "elapsed": 504,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 4082,
      "completion_tokens": 2,
      "total_tokens": 4084,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 4082
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "f8f7720b-d3a8-472a-90b9-ad8f44f4d46a",
    "object": "chat.completion",
    "created": 1790245076,
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
      "prompt_tokens": 4082,
      "completion_tokens": 2,
      "total_tokens": 4084,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 4082
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
