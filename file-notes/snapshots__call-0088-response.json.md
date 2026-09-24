# call-0088-response.json

> **路径**: `snapshots\call-0088-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.5 KB  
> **最后修改**: 2026-09-24T10:58:38.281Z  

## 文件开头预览

```json
{
  "callId": "call-0088",
  "timestamp": "2026-09-24T10-58-37-672Z",
  "elapsed": 608,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【110】】【【29】】【【18】】【【105】】【【123】】【【161】】【【162】】【【163】】【【165】】【【303】】【【306】】【【307】】【【344】】",
    "usage": {
      "prompt_tokens": 3561,
      "completion_tokens": 53,
      "total_tokens": 3614,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3561
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "f0ed331b-4ed5-40f6-b0bd-ec6bb1e69856",
    "object": "chat.completion",
    "created": 1790247517,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【110】】【【29】】【【18】】【【105】】【【123】】【【161】】【【162】】【【163】】【【165】】【【303】】【【306】】【【307】】【【344】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3561,
      "completion_tokens": 53,
      "total_tokens": 3614,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3561
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
