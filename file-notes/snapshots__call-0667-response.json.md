# call-0667-response.json

> **路径**: `snapshots\call-0667-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:17:59.407Z  

## 文件开头预览

```json
{
  "callId": "call-0667",
  "timestamp": "2026-09-24T10-17-58-914Z",
  "elapsed": 490,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【87】】【【88】】【【178】】",
    "usage": {
      "prompt_tokens": 3610,
      "completion_tokens": 13,
      "total_tokens": 3623,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3610
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "bf862782-02ad-48f9-90ff-88bd02644cad",
    "object": "chat.completion",
    "created": 1790245079,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【87】】【【88】】【【178】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3610,
      "completion_tokens": 13,
      "total_tokens": 3623,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3610
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
