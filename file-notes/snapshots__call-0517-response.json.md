# call-0517-response.json

> **路径**: `snapshots\call-0517-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:17:13.060Z  

## 文件开头预览

```json
{
  "callId": "call-0517",
  "timestamp": "2026-09-24T10-17-12-329Z",
  "elapsed": 730,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【91】】【【92】】【【93】】【【94】】【【96】】【【97】】【【281】】【【89】】【【184】】",
    "usage": {
      "prompt_tokens": 3478,
      "completion_tokens": 37,
      "total_tokens": 3515,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3478
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "49cd45d4-b37c-4fac-bcca-f2f160561b91",
    "object": "chat.completion",
    "created": 1790245032,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【91】】【【92】】【【93】】【【94】】【【96】】【【97】】【【281】】【【89】】【【184】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3478,
      "completion_tokens": 37,
      "total_tokens": 3515,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3478
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
