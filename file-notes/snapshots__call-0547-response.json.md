# call-0547-response.json

> **路径**: `snapshots\call-0547-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:17:34.679Z  

## 文件开头预览

```json
{
  "callId": "call-0547",
  "timestamp": "2026-09-24T10-17-33-899Z",
  "elapsed": 777,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【4】】【【8】】【【23】】【【40】】【【43】】【【45】】【【51】】【【54】】【【97】】【【340】】",
    "usage": {
      "prompt_tokens": 3789,
      "completion_tokens": 41,
      "total_tokens": 3830,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3789
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "11752b6b-a998-4740-b064-4fadf6897fcb",
    "object": "chat.completion",
    "created": 1790245054,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【4】】【【8】】【【23】】【【40】】【【43】】【【45】】【【51】】【【54】】【【97】】【【340】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3789,
      "completion_tokens": 41,
      "total_tokens": 3830,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3789
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
