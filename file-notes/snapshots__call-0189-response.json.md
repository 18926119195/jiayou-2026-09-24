# call-0189-response.json

> **路径**: `snapshots\call-0189-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:15:47.235Z  

## 文件开头预览

```json
{
  "callId": "call-0189",
  "timestamp": "2026-09-24T10-15-46-514Z",
  "elapsed": 719,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【8】】【【37】】【【63】】【【69】】【【88】】【【89】】【【284】】【【332】】",
    "usage": {
      "prompt_tokens": 3616,
      "completion_tokens": 33,
      "total_tokens": 3649,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3616
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "7f967670-e4fb-4810-bca6-4795c85236da",
    "object": "chat.completion",
    "created": 1790244946,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【8】】【【37】】【【63】】【【69】】【【88】】【【89】】【【284】】【【332】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3616,
      "completion_tokens": 33,
      "total_tokens": 3649,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3616
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
