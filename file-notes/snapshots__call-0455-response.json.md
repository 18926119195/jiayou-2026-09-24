# call-0455-response.json

> **路径**: `snapshots\call-0455-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:17:01.136Z  

## 文件开头预览

```json
{
  "callId": "call-0455",
  "timestamp": "2026-09-24T10-17-00-400Z",
  "elapsed": 732,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【6】】【【28】】【【29】】【【47】】【【51】】【【125】】【【173】】【【187】】【【203】】【【210】】【【215】】",
    "usage": {
      "prompt_tokens": 3853,
      "completion_tokens": 45,
      "total_tokens": 3898,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3853
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "02d238cb-884b-493e-bb36-ee267252c8e3",
    "object": "chat.completion",
    "created": 1790245020,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【6】】【【28】】【【29】】【【47】】【【51】】【【125】】【【173】】【【187】】【【203】】【【210】】【【215】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3853,
      "completion_tokens": 45,
      "total_tokens": 3898,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3853
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
