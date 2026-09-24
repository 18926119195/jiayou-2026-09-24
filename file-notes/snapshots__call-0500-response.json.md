# call-0500-response.json

> **路径**: `snapshots\call-0500-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:17:11.058Z  

## 文件开头预览

```json
{
  "callId": "call-0500",
  "timestamp": "2026-09-24T10-17-10-393Z",
  "elapsed": 664,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【175】】【【269】】【【321】】【【363】】【【421】】",
    "usage": {
      "prompt_tokens": 3952,
      "completion_tokens": 21,
      "total_tokens": 3973,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3952
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "2eab7444-c153-4c53-9d6d-d0d9f5ea0620",
    "object": "chat.completion",
    "created": 1790245030,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【175】】【【269】】【【321】】【【363】】【【421】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3952,
      "completion_tokens": 21,
      "total_tokens": 3973,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3952
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
