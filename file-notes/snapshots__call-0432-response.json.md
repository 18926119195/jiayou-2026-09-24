# call-0432-response.json

> **路径**: `snapshots\call-0432-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:16:51.323Z  

## 文件开头预览

```json
{
  "callId": "call-0432",
  "timestamp": "2026-09-24T10-16-50-497Z",
  "elapsed": 823,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【163】】【【209】】【【263】】【【266】】【【292】】",
    "usage": {
      "prompt_tokens": 3253,
      "completion_tokens": 21,
      "total_tokens": 3274,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3253
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "b4618df9-a178-4c18-9ad9-aaf1c766642a",
    "object": "chat.completion",
    "created": 1790245010,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【163】】【【209】】【【263】】【【266】】【【292】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3253,
      "completion_tokens": 21,
      "total_tokens": 3274,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3253
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
