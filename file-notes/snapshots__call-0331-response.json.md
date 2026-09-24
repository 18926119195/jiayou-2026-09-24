# call-0331-response.json

> **路径**: `snapshots\call-0331-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:16:24.556Z  

## 文件开头预览

```json
{
  "callId": "call-0331",
  "timestamp": "2026-09-24T10-16-24-058Z",
  "elapsed": 497,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3943,
      "completion_tokens": 2,
      "total_tokens": 3945,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3943
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "a94885eb-a39b-4e3a-9327-c351cf1c42db",
    "object": "chat.completion",
    "created": 1790244984,
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
      "prompt_tokens": 3943,
      "completion_tokens": 2,
      "total_tokens": 3945,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3943
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
