# call-0221-response.json

> **路径**: `snapshots\call-0221-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:15:49.870Z  

## 文件开头预览

```json
{
  "callId": "call-0221",
  "timestamp": "2026-09-24T10-15-49-376Z",
  "elapsed": 492,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【31】】【【74】】【【129】】【【137】】【【138】】【【161】】",
    "usage": {
      "prompt_tokens": 1683,
      "completion_tokens": 25,
      "total_tokens": 1708,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 1683
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "e36ef911-8524-4ef3-8bcc-4f06d2c363d5",
    "object": "chat.completion",
    "created": 1790244949,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【31】】【【74】】【【129】】【【137】】【【138】】【【161】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 1683,
      "completion_tokens": 25,
      "total_tokens": 1708,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 1683
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
