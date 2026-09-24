# call-0597-response.json

> **路径**: `snapshots\call-0597-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:45.952Z  

## 文件开头预览

```json
{
  "callId": "call-0597",
  "timestamp": "2026-09-24T10-17-45-447Z",
  "elapsed": 502,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3742,
      "completion_tokens": 2,
      "total_tokens": 3744,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3742
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "f1baf5ac-b461-44f8-a7dc-31e6222241c0",
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
      "prompt_tokens": 3742,
      "completion_tokens": 2,
      "total_tokens": 3744,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3742
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
