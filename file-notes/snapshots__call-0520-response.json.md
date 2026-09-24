# call-0520-response.json

> **路径**: `snapshots\call-0520-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:17:13.165Z  

## 文件开头预览

```json
{
  "callId": "call-0520",
  "timestamp": "2026-09-24T10-17-12-476Z",
  "elapsed": 688,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【75】】【【229】】【【93】】【【29】】【【34】】【【242】】",
    "usage": {
      "prompt_tokens": 3277,
      "completion_tokens": 25,
      "total_tokens": 3302,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3277
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "c3ab09f3-53f2-4b73-9106-f81b7d20be5f",
    "object": "chat.completion",
    "created": 1790245032,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【75】】【【229】】【【93】】【【29】】【【34】】【【242】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3277,
      "completion_tokens": 25,
      "total_tokens": 3302,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3277
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
