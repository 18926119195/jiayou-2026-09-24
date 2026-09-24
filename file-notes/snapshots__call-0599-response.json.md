# call-0599-response.json

> **路径**: `snapshots\call-0599-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:46.076Z  

## 文件开头预览

```json
{
  "callId": "call-0599",
  "timestamp": "2026-09-24T10-17-45-542Z",
  "elapsed": 531,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3462,
      "completion_tokens": 2,
      "total_tokens": 3464,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3462
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "716a9b69-93c3-4c95-a4f6-685a33650d50",
    "object": "chat.completion",
    "created": 1790245065,
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
      "prompt_tokens": 3462,
      "completion_tokens": 2,
      "total_tokens": 3464,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3462
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
