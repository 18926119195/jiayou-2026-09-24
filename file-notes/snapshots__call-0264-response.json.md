# call-0264-response.json

> **路径**: `snapshots\call-0264-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:16:01.278Z  

## 文件开头预览

```json
{
  "callId": "call-0264",
  "timestamp": "2026-09-24T10-16-00-378Z",
  "elapsed": 897,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【43】】【【189】】【【193】】【【197】】【【200】】【【204】】【【205】】【【263】】",
    "usage": {
      "prompt_tokens": 3105,
      "completion_tokens": 33,
      "total_tokens": 3138,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3105
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "0bd4c441-8d1f-4975-bbda-39f0832df75d",
    "object": "chat.completion",
    "created": 1790244960,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【43】】【【189】】【【193】】【【197】】【【200】】【【204】】【【205】】【【263】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3105,
      "completion_tokens": 33,
      "total_tokens": 3138,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3105
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
