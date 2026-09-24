# call-0097-response.json

> **路径**: `snapshots\call-0097-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:58:46.407Z  

## 文件开头预览

```json
{
  "callId": "call-0097",
  "timestamp": "2026-09-24T10-58-45-818Z",
  "elapsed": 587,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【50】】【【52】】【【53】】【【120】】【【130】】【【151】】【【323】】【【330】】【【342】】【【344】】",
    "usage": {
      "prompt_tokens": 3690,
      "completion_tokens": 41,
      "total_tokens": 3731,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3690
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "d48715c7-1dfc-40d2-83a4-9cff5057020b",
    "object": "chat.completion",
    "created": 1790247526,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【50】】【【52】】【【53】】【【120】】【【130】】【【151】】【【323】】【【330】】【【342】】【【344】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3690,
      "completion_tokens": 41,
      "total_tokens": 3731,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3690
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
