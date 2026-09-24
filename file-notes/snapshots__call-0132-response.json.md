# call-0132-response.json

> **路径**: `snapshots\call-0132-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:58:49.883Z  

## 文件开头预览

```json
{
  "callId": "call-0132",
  "timestamp": "2026-09-24T10-58-49-436Z",
  "elapsed": 445,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【89】】【【279】】【【313】】【【315】】【【330】】【【356】】",
    "usage": {
      "prompt_tokens": 3710,
      "completion_tokens": 25,
      "total_tokens": 3735,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3710
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "70e6cdb2-c027-44cf-b9bf-6b606db61e53",
    "object": "chat.completion",
    "created": 1790247529,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【89】】【【279】】【【313】】【【315】】【【330】】【【356】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3710,
      "completion_tokens": 25,
      "total_tokens": 3735,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3710
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
