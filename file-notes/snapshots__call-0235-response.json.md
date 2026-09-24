# call-0235-response.json

> **路径**: `snapshots\call-0235-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:15:58.320Z  

## 文件开头预览

```json
{
  "callId": "call-0235",
  "timestamp": "2026-09-24T10-15-57-678Z",
  "elapsed": 640,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3736,
      "completion_tokens": 2,
      "total_tokens": 3738,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3736
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "3d85bf28-a026-45eb-a68c-57aeed57defa",
    "object": "chat.completion",
    "created": 1790244957,
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
      "prompt_tokens": 3736,
      "completion_tokens": 2,
      "total_tokens": 3738,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3736
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
