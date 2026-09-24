# call-0590-response.json

> **路径**: `snapshots\call-0590-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:17:45.547Z  

## 文件开头预览

```json
{
  "callId": "call-0590",
  "timestamp": "2026-09-24T10-17-44-594Z",
  "elapsed": 950,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【19】】【【62】】【【103】】【【125】】【【173】】【【179】】【【203】】【【215】】",
    "usage": {
      "prompt_tokens": 3860,
      "completion_tokens": 33,
      "total_tokens": 3893,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3860
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "73a5ec0f-4db0-41e7-92cb-8b42232de650",
    "object": "chat.completion",
    "created": 1790245064,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【19】】【【62】】【【103】】【【125】】【【173】】【【179】】【【203】】【【215】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3860,
      "completion_tokens": 33,
      "total_tokens": 3893,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3860
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
