# call-0333-response.json

> **路径**: `snapshots\call-0333-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.5 KB  
> **最后修改**: 2026-09-24T10:16:24.754Z  

## 文件开头预览

```json
{
  "callId": "call-0333",
  "timestamp": "2026-09-24T10-16-24-243Z",
  "elapsed": 509,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【13】】【【14】】【【16】】【【17】】【【46】】【【47】】【【62】】【【63】】【【99】】【【260】】【【261】】【【333】】",
    "usage": {
      "prompt_tokens": 3986,
      "completion_tokens": 49,
      "total_tokens": 4035,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3986
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "7b2aa0a1-fadb-4f40-b52b-56229286666b",
    "object": "chat.completion",
    "created": 1790244984,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【13】】【【14】】【【16】】【【17】】【【46】】【【47】】【【62】】【【63】】【【99】】【【260】】【【261】】【【333】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3986,
      "completion_tokens": 49,
      "total_tokens": 4035,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3986
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
