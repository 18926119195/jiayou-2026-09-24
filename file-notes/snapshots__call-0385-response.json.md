# call-0385-response.json

> **路径**: `snapshots\call-0385-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:16:36.539Z  

## 文件开头预览

```json
{
  "callId": "call-0385",
  "timestamp": "2026-09-24T10-16-35-820Z",
  "elapsed": 716,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【54】】【【120】】【【252】】【【287】】",
    "usage": {
      "prompt_tokens": 3689,
      "completion_tokens": 17,
      "total_tokens": 3706,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3689
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "a2bfbc49-3ae9-49f7-87d1-7a6fb2fb11d9",
    "object": "chat.completion",
    "created": 1790244996,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【54】】【【120】】【【252】】【【287】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3689,
      "completion_tokens": 17,
      "total_tokens": 3706,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3689
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
