# call-0398-response.json

> **路径**: `snapshots\call-0398-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:16:37.581Z  

## 文件开头预览

```json
{
  "callId": "call-0398",
  "timestamp": "2026-09-24T10-16-36-967Z",
  "elapsed": 611,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【14】】【【26】】【【67】】【【92】】【【93】】【【250】】",
    "usage": {
      "prompt_tokens": 3421,
      "completion_tokens": 25,
      "total_tokens": 3446,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3421
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "4df64f6e-ef1c-4f3e-a948-97e768d1f7a2",
    "object": "chat.completion",
    "created": 1790244997,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【14】】【【26】】【【67】】【【92】】【【93】】【【250】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3421,
      "completion_tokens": 25,
      "total_tokens": 3446,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3421
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
