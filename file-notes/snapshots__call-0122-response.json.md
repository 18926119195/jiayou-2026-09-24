# call-0122-response.json

> **路径**: `snapshots\call-0122-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:58:49.325Z  

## 文件开头预览

```json
{
  "callId": "call-0122",
  "timestamp": "2026-09-24T10-58-48-511Z",
  "elapsed": 813,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【219】】【【239】】【【299】】【【270】】【【272】】【【373】】【【398】】【【399】】",
    "usage": {
      "prompt_tokens": 3985,
      "completion_tokens": 33,
      "total_tokens": 4018,
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
    "id": "0ef67222-87bb-406b-a0c5-9c7bfa157fc3",
    "object": "chat.completion",
    "created": 1790247528,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【219】】【【239】】【【299】】【【270】】【【272】】【【373】】【【398】】【【399】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3985,
      "completion_tokens": 33,
      "total_tokens": 4018,
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
