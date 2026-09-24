# call-0620-response.json

> **路径**: `snapshots\call-0620-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:17:47.826Z  

## 文件开头预览

```json
{
  "callId": "call-0620",
  "timestamp": "2026-09-24T10-17-47-386Z",
  "elapsed": 437,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【96】】【【174】】【【364】】",
    "usage": {
      "prompt_tokens": 3682,
      "completion_tokens": 13,
      "total_tokens": 3695,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3682
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "314b9c1f-af02-4ec7-a77f-28eef9f7a7ef",
    "object": "chat.completion",
    "created": 1790245067,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【96】】【【174】】【【364】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3682,
      "completion_tokens": 13,
      "total_tokens": 3695,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3682
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
