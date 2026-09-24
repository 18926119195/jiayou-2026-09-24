# call-0414-response.json

> **路径**: `snapshots\call-0414-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:16:49.884Z  

## 文件开头预览

```json
{
  "callId": "call-0414",
  "timestamp": "2026-09-24T10-16-49-267Z",
  "elapsed": 615,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3780,
      "completion_tokens": 2,
      "total_tokens": 3782,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3780
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "7ae4b38e-d267-40a9-b0fd-315a95a0ba69",
    "object": "chat.completion",
    "created": 1790245009,
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
      "prompt_tokens": 3780,
      "completion_tokens": 2,
      "total_tokens": 3782,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3780
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
