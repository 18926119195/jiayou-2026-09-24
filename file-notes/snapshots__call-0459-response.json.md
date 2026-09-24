# call-0459-response.json

> **路径**: `snapshots\call-0459-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:17:01.690Z  

## 文件开头预览

```json
{
  "callId": "call-0459",
  "timestamp": "2026-09-24T10-17-01-055Z",
  "elapsed": 632,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【6】】【【90】】【【255】】【【256】】",
    "usage": {
      "prompt_tokens": 3780,
      "completion_tokens": 17,
      "total_tokens": 3797,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3780
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "2c2409b8-b8ac-4a2c-95b3-adbea41d44b6",
    "object": "chat.completion",
    "created": 1790245021,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【6】】【【90】】【【255】】【【256】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3780,
      "completion_tokens": 17,
      "total_tokens": 3797,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3780
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
