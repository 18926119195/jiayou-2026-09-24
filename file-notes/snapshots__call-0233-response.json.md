# call-0233-response.json

> **路径**: `snapshots\call-0233-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:15:58.448Z  

## 文件开头预览

```json
{
  "callId": "call-0233",
  "timestamp": "2026-09-24T10-15-57-636Z",
  "elapsed": 809,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【13】】【【230】】【【243】】【【305】】",
    "usage": {
      "prompt_tokens": 3379,
      "completion_tokens": 17,
      "total_tokens": 3396,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3379
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "a6ed040b-fb9d-4b28-951e-ed13bc800d42",
    "object": "chat.completion",
    "created": 1790244957,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【13】】【【230】】【【243】】【【305】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3379,
      "completion_tokens": 17,
      "total_tokens": 3396,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3379
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
