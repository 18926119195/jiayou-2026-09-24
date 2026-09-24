# call-0083-response.json

> **路径**: `snapshots\call-0083-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:58:37.722Z  

## 文件开头预览

```json
{
  "callId": "call-0083",
  "timestamp": "2026-09-24T10-58-37-144Z",
  "elapsed": 577,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【58】】【【191】】【【220】】【【330】】【【331】】【【345】】",
    "usage": {
      "prompt_tokens": 3829,
      "completion_tokens": 25,
      "total_tokens": 3854,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3829
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "09103bcb-b96a-4324-858a-998149fb6072",
    "object": "chat.completion",
    "created": 1790247517,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【58】】【【191】】【【220】】【【330】】【【331】】【【345】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3829,
      "completion_tokens": 25,
      "total_tokens": 3854,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3829
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
