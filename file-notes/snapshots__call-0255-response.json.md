# call-0255-response.json

> **路径**: `snapshots\call-0255-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:16:00.115Z  

## 文件开头预览

```json
{
  "callId": "call-0255",
  "timestamp": "2026-09-24T10-15-59-480Z",
  "elapsed": 633,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【364】】【【365】】【【366】】",
    "usage": {
      "prompt_tokens": 3675,
      "completion_tokens": 13,
      "total_tokens": 3688,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3675
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "05d88a15-bb8a-422f-8d05-93840106c78b",
    "object": "chat.completion",
    "created": 1790244959,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【364】】【【365】】【【366】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3675,
      "completion_tokens": 13,
      "total_tokens": 3688,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3675
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
