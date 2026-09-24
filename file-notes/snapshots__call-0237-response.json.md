# call-0237-response.json

> **路径**: `snapshots\call-0237-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:15:58.815Z  

## 文件开头预览

```json
{
  "callId": "call-0237",
  "timestamp": "2026-09-24T10-15-57-956Z",
  "elapsed": 856,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【65】】【【71】】【【72】】【【73】】【【74】】【【75】】【【289】】【【306】】",
    "usage": {
      "prompt_tokens": 3456,
      "completion_tokens": 33,
      "total_tokens": 3489,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3456
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "87c6bce2-a909-47f4-bb6a-a526c04b4a9b",
    "object": "chat.completion",
    "created": 1790244958,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【65】】【【71】】【【72】】【【73】】【【74】】【【75】】【【289】】【【306】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3456,
      "completion_tokens": 33,
      "total_tokens": 3489,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3456
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
