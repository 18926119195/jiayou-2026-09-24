# call-0208-response.json

> **路径**: `snapshots\call-0208-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:15:48.897Z  

## 文件开头预览

```json
{
  "callId": "call-0208",
  "timestamp": "2026-09-24T10-15-48-086Z",
  "elapsed": 809,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【15】】【【50】】【【275】】【【332】】【【335】】",
    "usage": {
      "prompt_tokens": 3656,
      "completion_tokens": 21,
      "total_tokens": 3677,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3656
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "f6bdb7bc-dfa9-4dd9-942a-55c8f3c4f32b",
    "object": "chat.completion",
    "created": 1790244948,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【15】】【【50】】【【275】】【【332】】【【335】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3656,
      "completion_tokens": 21,
      "total_tokens": 3677,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3656
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
