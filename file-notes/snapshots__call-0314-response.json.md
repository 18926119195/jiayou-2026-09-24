# call-0314-response.json

> **路径**: `snapshots\call-0314-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.5 KB  
> **最后修改**: 2026-09-24T10:16:23.488Z  

## 文件开头预览

```json
{
  "callId": "call-0314",
  "timestamp": "2026-09-24T10-16-22-571Z",
  "elapsed": 916,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【25】】【【28】】【【37】】【【113】】【【125】】【【146】】【【182】】【【255】】【【300】】【【407】】【【429】】【【478】】",
    "usage": {
      "prompt_tokens": 4155,
      "completion_tokens": 49,
      "total_tokens": 4204,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 4155
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "495f664b-95e7-404a-a452-6d601c9ce293",
    "object": "chat.completion",
    "created": 1790244982,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【25】】【【28】】【【37】】【【113】】【【125】】【【146】】【【182】】【【255】】【【300】】【【407】】【【429】】【【478】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 4155,
      "completion_tokens": 49,
      "total_tokens": 4204,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 4155
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
