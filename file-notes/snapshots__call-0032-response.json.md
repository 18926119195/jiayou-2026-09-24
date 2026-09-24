# call-0032-response.json

> **路径**: `snapshots\call-0032-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T12:14:13.247Z  

## 文件开头预览

```json
{
  "callId": "call-0032",
  "timestamp": "2026-09-24T12-14-12-714Z",
  "elapsed": 533,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【95】】【【250】】",
    "usage": {
      "prompt_tokens": 3657,
      "completion_tokens": 9,
      "total_tokens": 3666,
      "prompt_tokens_details": {
        "cached_tokens": 3456
      },
      "prompt_cache_hit_tokens": 3456,
      "prompt_cache_miss_tokens": 201
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "7855a797-392b-4ab4-a7be-7443b464d89c",
    "object": "chat.completion",
    "created": 1790252052,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【95】】【【250】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3657,
      "completion_tokens": 9,
      "total_tokens": 3666,
      "prompt_tokens_details": {
        "cached_tokens": 3456
      },
      "prompt_cache_hit_tokens": 3456,
      "prompt_cache_miss_tokens": 201
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
