# call-0528-response.json

> **路径**: `snapshots\call-0528-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:17:14.171Z  

## 文件开头预览

```json
{
  "callId": "call-0528",
  "timestamp": "2026-09-24T10-17-13-444Z",
  "elapsed": 725,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【55】】【【290】】【【373】】",
    "usage": {
      "prompt_tokens": 3857,
      "completion_tokens": 13,
      "total_tokens": 3870,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3857
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "7b3d907a-66cf-48a9-9e6f-7a46e9b178c7",
    "object": "chat.completion",
    "created": 1790245033,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【55】】【【290】】【【373】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3857,
      "completion_tokens": 13,
      "total_tokens": 3870,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3857
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
