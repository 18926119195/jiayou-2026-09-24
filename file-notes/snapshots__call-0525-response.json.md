# call-0525-response.json

> **路径**: `snapshots\call-0525-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:17:13.453Z  

## 文件开头预览

```json
{
  "callId": "call-0525",
  "timestamp": "2026-09-24T10-17-13-060Z",
  "elapsed": 392,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【2】】【【30】】【【74】】【【75】】【【114】】【【184】】【【331】】【【332】】",
    "usage": {
      "prompt_tokens": 3733,
      "completion_tokens": 33,
      "total_tokens": 3766,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3733
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "1f50882b-0233-48d7-83ca-a98a5c6fa84d",
    "object": "chat.completion",
    "created": 1790245033,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【2】】【【30】】【【74】】【【75】】【【114】】【【184】】【【331】】【【332】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3733,
      "completion_tokens": 33,
      "total_tokens": 3766,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3733
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
