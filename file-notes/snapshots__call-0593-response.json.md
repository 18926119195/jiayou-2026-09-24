# call-0593-response.json

> **路径**: `snapshots\call-0593-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:17:45.348Z  

## 文件开头预览

```json
{
  "callId": "call-0593",
  "timestamp": "2026-09-24T10-17-44-595Z",
  "elapsed": 750,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【20】】【【319】】",
    "usage": {
      "prompt_tokens": 3771,
      "completion_tokens": 9,
      "total_tokens": 3780,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3771
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "efd8d990-7e7a-4078-849f-bcf3c93ea3b6",
    "object": "chat.completion",
    "created": 1790245064,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【20】】【【319】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3771,
      "completion_tokens": 9,
      "total_tokens": 3780,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3771
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
