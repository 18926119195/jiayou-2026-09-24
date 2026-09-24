# call-0550-response.json

> **路径**: `snapshots\call-0550-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.6 KB  
> **最后修改**: 2026-09-24T10:17:35.496Z  

## 文件开头预览

```json
{
  "callId": "call-0550",
  "timestamp": "2026-09-24T10-17-34-580Z",
  "elapsed": 913,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【215】】【【300】】【【67】】【【70】】【【123】】【【141】】【【151】】【【41】】【【53】】【【57】】【【138】】【【142】】【【150】】【【185】】【【290】】【【305】】",
    "usage": {
      "prompt_tokens": 3381,
      "completion_tokens": 65,
      "total_tokens": 3446,
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
    "id": "36e25189-959b-495b-b9e0-1963bc98753f",
    "object": "chat.completion",
    "created": 1790245054,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【215】】【【300】】【【67】】【【70】】【【123】】【【141】】【【151】】【【41】】【【53】】【【57】】【【138】】【【142】】【【150】】【【185】】【【290】】【【305】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3381,
      "completion_tokens": 65,
      "total_tokens": 3446,
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
