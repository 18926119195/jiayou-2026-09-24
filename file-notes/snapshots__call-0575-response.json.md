# call-0575-response.json

> **路径**: `snapshots\call-0575-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.5 KB  
> **最后修改**: 2026-09-24T10:17:37.908Z  

## 文件开头预览

```json
{
  "callId": "call-0575",
  "timestamp": "2026-09-24T10-17-36-756Z",
  "elapsed": 1149,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【119】】【【121】】【【122】】【【120】】【【124】】【【174】】【【52】】【【89】】【【26】】【【279】】【【253】】【【301】】【【364】】【【370】】",
    "usage": {
      "prompt_tokens": 3678,
      "completion_tokens": 57,
      "total_tokens": 3735,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3678
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "b36242ab-be6b-4dbf-a3d9-e5712c1ca535",
    "object": "chat.completion",
    "created": 1790245056,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【119】】【【121】】【【122】】【【120】】【【124】】【【174】】【【52】】【【89】】【【26】】【【279】】【【253】】【【301】】【【364】】【【370】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3678,
      "completion_tokens": 57,
      "total_tokens": 3735,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3678
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
