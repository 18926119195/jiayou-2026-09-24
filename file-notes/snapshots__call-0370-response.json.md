# call-0370-response.json

> **路径**: `snapshots\call-0370-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:16:35.464Z  

## 文件开头预览

```json
{
  "callId": "call-0370",
  "timestamp": "2026-09-24T10-16-34-719Z",
  "elapsed": 744,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【13】】【【230】】【【305】】",
    "usage": {
      "prompt_tokens": 3386,
      "completion_tokens": 13,
      "total_tokens": 3399,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3386
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "1d14befa-1e5c-43ef-b81b-0bafc1b006ce",
    "object": "chat.completion",
    "created": 1790244995,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【13】】【【230】】【【305】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3386,
      "completion_tokens": 13,
      "total_tokens": 3399,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3386
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
