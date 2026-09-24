# call-0203-response.json

> **路径**: `snapshots\call-0203-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.6 KB  
> **最后修改**: 2026-09-24T10:15:48.370Z  

## 文件开头预览

```json
{
  "callId": "call-0203",
  "timestamp": "2026-09-24T10-15-47-547Z",
  "elapsed": 820,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【221】】【【253】】【【219】】【【230】】【【252】】【【287】】【【120】】【【54】】【【34】】【【222】】【【223】】【【210】】【【247】】【【116】】【【127】】【【297】】【【81】】",
    "usage": {
      "prompt_tokens": 3684,
      "completion_tokens": 69,
      "total_tokens": 3753,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3684
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "8774e415-9acc-4e10-ab34-05bc7f11325e",
    "object": "chat.completion",
    "created": 1790244947,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【221】】【【253】】【【219】】【【230】】【【252】】【【287】】【【120】】【【54】】【【34】】【【222】】【【223】】【【210】】【【247】】【【116】】【【127】】【【297】】【【81】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3684,
      "completion_tokens": 69,
      "total_tokens": 3753,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3684
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
