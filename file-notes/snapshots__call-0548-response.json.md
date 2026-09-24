# call-0548-response.json

> **路径**: `snapshots\call-0548-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:17:34.601Z  

## 文件开头预览

```json
{
  "callId": "call-0548",
  "timestamp": "2026-09-24T10-17-33-900Z",
  "elapsed": 699,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【20】】【【53】】【【54】】【【55】】【【56】】【【57】】【【58】】【【319】】",
    "usage": {
      "prompt_tokens": 3767,
      "completion_tokens": 33,
      "total_tokens": 3800,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3767
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "35c5e83c-53de-4865-88a7-22d89087672b",
    "object": "chat.completion",
    "created": 1790245054,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【20】】【【53】】【【54】】【【55】】【【56】】【【57】】【【58】】【【319】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3767,
      "completion_tokens": 33,
      "total_tokens": 3800,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3767
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
