# call-0188-response.json

> **路径**: `snapshots\call-0188-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:15:47.213Z  

## 文件开头预览

```json
{
  "callId": "call-0188",
  "timestamp": "2026-09-24T10-15-46-470Z",
  "elapsed": 741,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【13】】【【230】】【【231】】【【44】】【【45】】【【174】】【【298】】【【299】】【【300】】【【310】】【【311】】",
    "usage": {
      "prompt_tokens": 3381,
      "completion_tokens": 45,
      "total_tokens": 3426,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3381
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "9bfe41c6-bf1b-46d4-9f5a-dfafebb4224c",
    "object": "chat.completion",
    "created": 1790244946,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【13】】【【230】】【【231】】【【44】】【【45】】【【174】】【【298】】【【299】】【【300】】【【310】】【【311】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3381,
      "completion_tokens": 45,
      "total_tokens": 3426,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3381
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
