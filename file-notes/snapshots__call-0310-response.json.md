# call-0310-response.json

> **路径**: `snapshots\call-0310-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:16:13.266Z  

## 文件开头预览

```json
{
  "callId": "call-0310",
  "timestamp": "2026-09-24T10-16-12-668Z",
  "elapsed": 596,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【19】】【【21】】【【92】】【【95】】【【111】】【【118】】【【119】】【【138】】【【140】】【【145】】【【146】】",
    "usage": {
      "prompt_tokens": 1688,
      "completion_tokens": 45,
      "total_tokens": 1733,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 1688
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "1c72aa26-983e-4926-964e-cae13b3f843b",
    "object": "chat.completion",
    "created": 1790244972,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【19】】【【21】】【【92】】【【95】】【【111】】【【118】】【【119】】【【138】】【【140】】【【145】】【【146】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 1688,
      "completion_tokens": 45,
      "total_tokens": 1733,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 1688
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
