# call-0489-response.json

> **路径**: `snapshots\call-0489-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:17:04.251Z  

## 文件开头预览

```json
{
  "callId": "call-0489",
  "timestamp": "2026-09-24T10-17-03-617Z",
  "elapsed": 630,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【121】】【【160】】【【189】】【【276】】【【290】】【【313】】",
    "usage": {
      "prompt_tokens": 3483,
      "completion_tokens": 25,
      "total_tokens": 3508,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3483
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "09af88c5-2218-4f22-b047-efb0ec6e900c",
    "object": "chat.completion",
    "created": 1790245023,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【121】】【【160】】【【189】】【【276】】【【290】】【【313】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3483,
      "completion_tokens": 25,
      "total_tokens": 3508,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3483
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
