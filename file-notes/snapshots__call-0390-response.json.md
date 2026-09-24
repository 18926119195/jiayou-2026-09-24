# call-0390-response.json

> **路径**: `snapshots\call-0390-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:16:36.897Z  

## 文件开头预览

```json
{
  "callId": "call-0390",
  "timestamp": "2026-09-24T10-16-36-140Z",
  "elapsed": 755,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【15】】【【50】】【【85】】【【126】】【【275】】【【290】】",
    "usage": {
      "prompt_tokens": 3661,
      "completion_tokens": 25,
      "total_tokens": 3686,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3661
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "8ff53d65-1d88-4292-98aa-bc40d66c7798",
    "object": "chat.completion",
    "created": 1790244996,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【15】】【【50】】【【85】】【【126】】【【275】】【【290】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3661,
      "completion_tokens": 25,
      "total_tokens": 3686,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3661
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
