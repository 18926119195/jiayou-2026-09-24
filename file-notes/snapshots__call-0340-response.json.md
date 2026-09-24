# call-0340-response.json

> **路径**: `snapshots\call-0340-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:16:25.564Z  

## 文件开头预览

```json
{
  "callId": "call-0340",
  "timestamp": "2026-09-24T10-16-24-828Z",
  "elapsed": 735,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【73】】【【79】】【【87】】【【140】】【【142】】【【158】】【【178】】【【198】】【【251】】【【252】】",
    "usage": {
      "prompt_tokens": 3254,
      "completion_tokens": 41,
      "total_tokens": 3295,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3254
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "bbbafd89-c5df-4f6f-8703-6b65c344c4e9",
    "object": "chat.completion",
    "created": 1790244985,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【73】】【【79】】【【87】】【【140】】【【142】】【【158】】【【178】】【【198】】【【251】】【【252】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3254,
      "completion_tokens": 41,
      "total_tokens": 3295,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3254
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
