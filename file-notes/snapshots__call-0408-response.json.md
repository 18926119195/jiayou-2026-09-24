# call-0408-response.json

> **路径**: `snapshots\call-0408-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:16:49.279Z  

## 文件开头预览

```json
{
  "callId": "call-0408",
  "timestamp": "2026-09-24T10-16-48-552Z",
  "elapsed": 725,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【234】】【【237】】【【247】】【【309】】【【322】】【【382】】【【406】】【【414】】",
    "usage": {
      "prompt_tokens": 4053,
      "completion_tokens": 33,
      "total_tokens": 4086,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 4053
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "24195424-4ba1-4ad3-8734-3009bab0a0c4",
    "object": "chat.completion",
    "created": 1790245008,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【234】】【【237】】【【247】】【【309】】【【322】】【【382】】【【406】】【【414】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 4053,
      "completion_tokens": 33,
      "total_tokens": 4086,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 4053
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
