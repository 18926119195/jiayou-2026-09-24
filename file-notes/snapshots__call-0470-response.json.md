# call-0470-response.json

> **路径**: `snapshots\call-0470-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:17:03.437Z  

## 文件开头预览

```json
{
  "callId": "call-0470",
  "timestamp": "2026-09-24T10-17-01-776Z",
  "elapsed": 1658,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【13】】【【14】】【【46】】【【47】】【【99】】",
    "usage": {
      "prompt_tokens": 3985,
      "completion_tokens": 21,
      "total_tokens": 4006,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3985
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "a878c56b-2a44-444b-9ffe-6f9aee3083de",
    "object": "chat.completion",
    "created": 1790245023,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【13】】【【14】】【【46】】【【47】】【【99】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3985,
      "completion_tokens": 21,
      "total_tokens": 4006,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3985
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
