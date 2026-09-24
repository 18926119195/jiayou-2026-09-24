# call-0279-response.json

> **路径**: `snapshots\call-0279-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:16:09.837Z  

## 文件开头预览

```json
{
  "callId": "call-0279",
  "timestamp": "2026-09-24T10-16-09-433Z",
  "elapsed": 403,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3743,
      "completion_tokens": 2,
      "total_tokens": 3745,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3743
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "b68009e2-00a3-4d90-9b67-b2349f4ca321",
    "object": "chat.completion",
    "created": 1790244969,
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
      "prompt_tokens": 3743,
      "completion_tokens": 2,
      "total_tokens": 3745,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3743
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
