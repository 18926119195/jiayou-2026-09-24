# call-0469-response.json

> **路径**: `snapshots\call-0469-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:02.767Z  

## 文件开头预览

```json
{
  "callId": "call-0469",
  "timestamp": "2026-09-24T10-17-01-688Z",
  "elapsed": 1076,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3956,
      "completion_tokens": 2,
      "total_tokens": 3958,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3956
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "e67e9083-3556-4684-9ecf-3e4d37881194",
    "object": "chat.completion",
    "created": 1790245022,
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
      "prompt_tokens": 3956,
      "completion_tokens": 2,
      "total_tokens": 3958,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3956
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
