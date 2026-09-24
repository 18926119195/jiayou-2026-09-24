# call-0661-response.json

> **路径**: `snapshots\call-0661-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:17:59.009Z  

## 文件开头预览

```json
{
  "callId": "call-0661",
  "timestamp": "2026-09-24T10-17-58-473Z",
  "elapsed": 534,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【50】】【【55】】【【184】】",
    "usage": {
      "prompt_tokens": 3738,
      "completion_tokens": 13,
      "total_tokens": 3751,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3738
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "66e9907a-aa25-4162-87eb-8d058957e64d",
    "object": "chat.completion",
    "created": 1790245078,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【50】】【【55】】【【184】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3738,
      "completion_tokens": 13,
      "total_tokens": 3751,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3738
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
