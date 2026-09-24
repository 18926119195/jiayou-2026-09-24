# call-0400-response.json

> **路径**: `snapshots\call-0400-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:16:37.917Z  

## 文件开头预览

```json
{
  "callId": "call-0400",
  "timestamp": "2026-09-24T10-16-37-024Z",
  "elapsed": 891,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【54】】【【117】】【【140】】【【215】】【【247】】【【248】】",
    "usage": {
      "prompt_tokens": 3278,
      "completion_tokens": 25,
      "total_tokens": 3303,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3278
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "be4247cd-af2a-4d49-ad3c-b4e583e272ab",
    "object": "chat.completion",
    "created": 1790244997,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【54】】【【117】】【【140】】【【215】】【【247】】【【248】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3278,
      "completion_tokens": 25,
      "total_tokens": 3303,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3278
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
