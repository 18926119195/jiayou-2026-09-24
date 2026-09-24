# call-0483-response.json

> **路径**: `snapshots\call-0483-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:17:03.911Z  

## 文件开头预览

```json
{
  "callId": "call-0483",
  "timestamp": "2026-09-24T10-17-03-128Z",
  "elapsed": 780,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【3】】【【81】】【【323】】",
    "usage": {
      "prompt_tokens": 3494,
      "completion_tokens": 13,
      "total_tokens": 3507,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3494
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "faebef04-3f46-45e6-8cf6-798a701848ad",
    "object": "chat.completion",
    "created": 1790245023,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【3】】【【81】】【【323】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3494,
      "completion_tokens": 13,
      "total_tokens": 3507,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3494
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
