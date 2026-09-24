# call-0075-response.json

> **路径**: `snapshots\call-0075-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:58:37.145Z  

## 文件开头预览

```json
{
  "callId": "call-0075",
  "timestamp": "2026-09-24T10-58-36-546Z",
  "elapsed": 597,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【135】】【【298】】【【304】】【【305】】【【308】】【【349】】",
    "usage": {
      "prompt_tokens": 3714,
      "completion_tokens": 25,
      "total_tokens": 3739,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3714
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "7e269410-c9c3-4939-8221-e238e393ab5e",
    "object": "chat.completion",
    "created": 1790247516,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【135】】【【298】】【【304】】【【305】】【【308】】【【349】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3714,
      "completion_tokens": 25,
      "total_tokens": 3739,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3714
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
