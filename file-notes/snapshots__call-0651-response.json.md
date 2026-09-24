# call-0651-response.json

> **路径**: `snapshots\call-0651-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:58.305Z  

## 文件开头预览

```json
{
  "callId": "call-0651",
  "timestamp": "2026-09-24T10-17-57-736Z",
  "elapsed": 566,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 4032,
      "completion_tokens": 2,
      "total_tokens": 4034,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 4032
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "87114606-439f-440c-a65f-7d1bb62b31bf",
    "object": "chat.completion",
    "created": 1790245077,
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
      "prompt_tokens": 4032,
      "completion_tokens": 2,
      "total_tokens": 4034,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 4032
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
