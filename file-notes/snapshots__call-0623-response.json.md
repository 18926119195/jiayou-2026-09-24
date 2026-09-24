# call-0623-response.json

> **路径**: `snapshots\call-0623-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:17:48.293Z  

## 文件开头预览

```json
{
  "callId": "call-0623",
  "timestamp": "2026-09-24T10-17-47-568Z",
  "elapsed": 722,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【275】】",
    "usage": {
      "prompt_tokens": 3420,
      "completion_tokens": 5,
      "total_tokens": 3425,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3420
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "52c57706-901f-4bf8-a2ad-87bf68962169",
    "object": "chat.completion",
    "created": 1790245067,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【275】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3420,
      "completion_tokens": 5,
      "total_tokens": 3425,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3420
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
