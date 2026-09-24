# call-0615-response.json

> **路径**: `snapshots\call-0615-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:17:47.523Z  

## 文件开头预览

```json
{
  "callId": "call-0615",
  "timestamp": "2026-09-24T10-17-47-032Z",
  "elapsed": 488,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【15】】【【50】】【【275】】",
    "usage": {
      "prompt_tokens": 3660,
      "completion_tokens": 13,
      "total_tokens": 3673,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3660
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "948d361c-b1a4-4bb5-a529-eb46f3ac7762",
    "object": "chat.completion",
    "created": 1790245067,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【15】】【【50】】【【275】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3660,
      "completion_tokens": 13,
      "total_tokens": 3673,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3660
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
