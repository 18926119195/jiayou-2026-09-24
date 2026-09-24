# call-0320-response.json

> **路径**: `snapshots\call-0320-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:16:23.134Z  

## 文件开头预览

```json
{
  "callId": "call-0320",
  "timestamp": "2026-09-24T10-16-22-574Z",
  "elapsed": 558,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【4】】【【23】】【【43】】【【90】】【【104】】【【285】】【【290】】【【321】】",
    "usage": {
      "prompt_tokens": 3787,
      "completion_tokens": 33,
      "total_tokens": 3820,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3787
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "090172e9-4173-4896-babe-7af3cc2e7826",
    "object": "chat.completion",
    "created": 1790244982,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【4】】【【23】】【【43】】【【90】】【【104】】【【285】】【【290】】【【321】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3787,
      "completion_tokens": 33,
      "total_tokens": 3820,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3787
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
