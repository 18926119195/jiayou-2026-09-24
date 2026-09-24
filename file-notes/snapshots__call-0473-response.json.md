# call-0473-response.json

> **路径**: `snapshots\call-0473-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:17:02.823Z  

## 文件开头预览

```json
{
  "callId": "call-0473",
  "timestamp": "2026-09-24T10-17-02-043Z",
  "elapsed": 777,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【45】】【【71】】【【92】】【【138】】【【287】】",
    "usage": {
      "prompt_tokens": 3480,
      "completion_tokens": 21,
      "total_tokens": 3501,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3480
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "89e39176-99e5-4622-bc3f-7c6faaa86c9c",
    "object": "chat.completion",
    "created": 1790245022,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【45】】【【71】】【【92】】【【138】】【【287】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3480,
      "completion_tokens": 21,
      "total_tokens": 3501,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3480
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
