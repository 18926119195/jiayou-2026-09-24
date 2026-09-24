# call-0332-response.json

> **路径**: `snapshots\call-0332-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:16:24.829Z  

## 文件开头预览

```json
{
  "callId": "call-0332",
  "timestamp": "2026-09-24T10-16-24-184Z",
  "elapsed": 644,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【31】】【【93】】【【125】】【【128】】【【216】】【【235】】【【236】】【【357】】",
    "usage": {
      "prompt_tokens": 3957,
      "completion_tokens": 33,
      "total_tokens": 3990,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3957
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "16eb8ba6-c74c-4d4d-a30e-836e5053c696",
    "object": "chat.completion",
    "created": 1790244984,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【31】】【【93】】【【125】】【【128】】【【216】】【【235】】【【236】】【【357】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3957,
      "completion_tokens": 33,
      "total_tokens": 3990,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3957
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
