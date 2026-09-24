# call-0204-response.json

> **路径**: `snapshots\call-0204-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:15:48.076Z  

## 文件开头预览

```json
{
  "callId": "call-0204",
  "timestamp": "2026-09-24T10-15-47-550Z",
  "elapsed": 524,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【43】】【【151】】【【227】】【【244】】【【245】】【【259】】【【276】】【【305】】",
    "usage": {
      "prompt_tokens": 3282,
      "completion_tokens": 33,
      "total_tokens": 3315,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3282
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "98934a10-4586-451b-8bdf-855e2d653b7a",
    "object": "chat.completion",
    "created": 1790244947,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【43】】【【151】】【【227】】【【244】】【【245】】【【259】】【【276】】【【305】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3282,
      "completion_tokens": 33,
      "total_tokens": 3315,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3282
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
