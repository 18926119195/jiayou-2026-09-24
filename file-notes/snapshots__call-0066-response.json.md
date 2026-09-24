# call-0066-response.json

> **路径**: `snapshots\call-0066-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:58:36.547Z  

## 文件开头预览

```json
{
  "callId": "call-0066",
  "timestamp": "2026-09-24T10-58-35-872Z",
  "elapsed": 672,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【112】】【【210】】【【243】】【【372】】",
    "usage": {
      "prompt_tokens": 3765,
      "completion_tokens": 17,
      "total_tokens": 3782,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3765
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "be28240f-be7b-4623-afc1-c064319ccc45",
    "object": "chat.completion",
    "created": 1790247516,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【112】】【【210】】【【243】】【【372】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3765,
      "completion_tokens": 17,
      "total_tokens": 3782,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3765
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
