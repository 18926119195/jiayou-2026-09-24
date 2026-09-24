# call-0670-response.json

> **路径**: `snapshots\call-0670-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:59.485Z  

## 文件开头预览

```json
{
  "callId": "call-0670",
  "timestamp": "2026-09-24T10-17-59-007Z",
  "elapsed": 475,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3273,
      "completion_tokens": 2,
      "total_tokens": 3275,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3273
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "581c9922-cc5b-4f86-ba52-e07e830c3f46",
    "object": "chat.completion",
    "created": 1790245079,
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
      "prompt_tokens": 3273,
      "completion_tokens": 2,
      "total_tokens": 3275,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3273
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
