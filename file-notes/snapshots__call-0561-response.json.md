# call-0561-response.json

> **路径**: `snapshots\call-0561-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:17:36.333Z  

## 文件开头预览

```json
{
  "callId": "call-0561",
  "timestamp": "2026-09-24T10-17-35-494Z",
  "elapsed": 837,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【136】】【【226】】【【227】】【【228】】【【335】】",
    "usage": {
      "prompt_tokens": 4032,
      "completion_tokens": 21,
      "total_tokens": 4053,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 4032
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "831e7802-c814-4205-bae7-f5f907352173",
    "object": "chat.completion",
    "created": 1790245055,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【136】】【【226】】【【227】】【【228】】【【335】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 4032,
      "completion_tokens": 21,
      "total_tokens": 4053,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 4032
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
