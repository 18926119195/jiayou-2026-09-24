# call-0197-response.json

> **路径**: `snapshots\call-0197-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:15:48.279Z  

## 文件开头预览

```json
{
  "callId": "call-0197",
  "timestamp": "2026-09-24T10-15-47-193Z",
  "elapsed": 1084,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【17】】【【18】】",
    "usage": {
      "prompt_tokens": 3959,
      "completion_tokens": 9,
      "total_tokens": 3968,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3959
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "088157c8-4f06-488f-8be4-7f8f71940b0e",
    "object": "chat.completion",
    "created": 1790244947,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【17】】【【18】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3959,
      "completion_tokens": 9,
      "total_tokens": 3968,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3959
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
