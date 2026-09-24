# call-0632-response.json

> **路径**: `snapshots\call-0632-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:17:57.174Z  

## 文件开头预览

```json
{
  "callId": "call-0632",
  "timestamp": "2026-09-24T10-17-56-543Z",
  "elapsed": 626,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【204】】【【259】】【【134】】【【229】】【【318】】",
    "usage": {
      "prompt_tokens": 4062,
      "completion_tokens": 21,
      "total_tokens": 4083,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 4062
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "59c19a4a-8b54-4111-8a6f-e80c596cd888",
    "object": "chat.completion",
    "created": 1790245076,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【204】】【【259】】【【134】】【【229】】【【318】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 4062,
      "completion_tokens": 21,
      "total_tokens": 4083,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 4062
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
