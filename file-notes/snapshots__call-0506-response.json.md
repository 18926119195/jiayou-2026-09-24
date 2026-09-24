# call-0506-response.json

> **路径**: `snapshots\call-0506-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:17:11.653Z  

## 文件开头预览

```json
{
  "callId": "call-0506",
  "timestamp": "2026-09-24T10-17-11-057Z",
  "elapsed": 593,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【62】】【【266】】",
    "usage": {
      "prompt_tokens": 3733,
      "completion_tokens": 9,
      "total_tokens": 3742,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3733
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "711c8a37-4395-445c-84dd-4db04a2a6998",
    "object": "chat.completion",
    "created": 1790245031,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【62】】【【266】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3733,
      "completion_tokens": 9,
      "total_tokens": 3742,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3733
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
