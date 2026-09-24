# call-0293-response.json

> **路径**: `snapshots\call-0293-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:16:11.478Z  

## 文件开头预览

```json
{
  "callId": "call-0293",
  "timestamp": "2026-09-24T10-16-10-698Z",
  "elapsed": 779,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【43】】【【227】】【【276】】【【285】】【【290】】【【305】】",
    "usage": {
      "prompt_tokens": 3287,
      "completion_tokens": 25,
      "total_tokens": 3312,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3287
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "edcdc0bb-cb9a-40b8-9245-a5a6a606ba24",
    "object": "chat.completion",
    "created": 1790244970,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【43】】【【227】】【【276】】【【285】】【【290】】【【305】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3287,
      "completion_tokens": 25,
      "total_tokens": 3312,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3287
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
