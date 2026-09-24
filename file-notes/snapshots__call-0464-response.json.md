# call-0464-response.json

> **路径**: `snapshots\call-0464-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:17:02.045Z  

## 文件开头预览

```json
{
  "callId": "call-0464",
  "timestamp": "2026-09-24T10-17-01-253Z",
  "elapsed": 789,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【5】】【【6】】【【7】】【【41】】【【42】】【【203】】【【263】】【【264】】【【289】】【【306】】",
    "usage": {
      "prompt_tokens": 3455,
      "completion_tokens": 41,
      "total_tokens": 3496,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3455
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "2eb158c2-9343-4dff-80c5-d6250f4f3364",
    "object": "chat.completion",
    "created": 1790245021,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【5】】【【6】】【【7】】【【41】】【【42】】【【203】】【【263】】【【264】】【【289】】【【306】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3455,
      "completion_tokens": 41,
      "total_tokens": 3496,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3455
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
