# call-0371-response.json

> **路径**: `snapshots\call-0371-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:16:35.589Z  

## 文件开头预览

```json
{
  "callId": "call-0371",
  "timestamp": "2026-09-24T10-16-34-784Z",
  "elapsed": 803,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【6】】【【8】】【【25】】【【28】】【【52】】【【57】】【【332】】",
    "usage": {
      "prompt_tokens": 3621,
      "completion_tokens": 29,
      "total_tokens": 3650,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3621
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "ed382778-039f-4a05-874c-a1f0817a2df0",
    "object": "chat.completion",
    "created": 1790244995,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【6】】【【8】】【【25】】【【28】】【【52】】【【57】】【【332】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3621,
      "completion_tokens": 29,
      "total_tokens": 3650,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3621
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
