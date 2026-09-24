# call-0325-response.json

> **路径**: `snapshots\call-0325-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:16:24.013Z  

## 文件开头预览

```json
{
  "callId": "call-0325",
  "timestamp": "2026-09-24T10-16-23-379Z",
  "elapsed": 633,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【101】】【【102】】【【103】】【【118】】【【119】】【【120】】【【137】】【【153】】【【214】】【【252】】【【262】】",
    "usage": {
      "prompt_tokens": 3736,
      "completion_tokens": 45,
      "total_tokens": 3781,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3736
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "6e3e350a-999f-46b4-8d50-6298c0726d53",
    "object": "chat.completion",
    "created": 1790244983,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【101】】【【102】】【【103】】【【118】】【【119】】【【120】】【【137】】【【153】】【【214】】【【252】】【【262】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3736,
      "completion_tokens": 45,
      "total_tokens": 3781,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3736
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
