# call-0481-response.json

> **路径**: `snapshots\call-0481-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:17:03.622Z  

## 文件开头预览

```json
{
  "callId": "call-0481",
  "timestamp": "2026-09-24T10-17-02-877Z",
  "elapsed": 741,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【50】】【【55】】【【59】】",
    "usage": {
      "prompt_tokens": 3735,
      "completion_tokens": 13,
      "total_tokens": 3748,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3735
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "20b9ee4b-751d-4296-8329-7d87c499f541",
    "object": "chat.completion",
    "created": 1790245023,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【50】】【【55】】【【59】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3735,
      "completion_tokens": 13,
      "total_tokens": 3748,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3735
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
