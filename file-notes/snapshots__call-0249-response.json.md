# call-0249-response.json

> **路径**: `snapshots\call-0249-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:15:59.724Z  

## 文件开头预览

```json
{
  "callId": "call-0249",
  "timestamp": "2026-09-24T10-15-59-012Z",
  "elapsed": 708,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【43】】【【73】】【【227】】【【290】】【【295】】",
    "usage": {
      "prompt_tokens": 3280,
      "completion_tokens": 21,
      "total_tokens": 3301,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3280
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "96a72a46-4766-426a-a753-755a98dd4ef8",
    "object": "chat.completion",
    "created": 1790244959,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【43】】【【73】】【【227】】【【290】】【【295】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3280,
      "completion_tokens": 21,
      "total_tokens": 3301,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3280
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
