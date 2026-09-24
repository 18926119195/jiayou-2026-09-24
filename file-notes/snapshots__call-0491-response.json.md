# call-0491-response.json

> **路径**: `snapshots\call-0491-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.5 KB  
> **最后修改**: 2026-09-24T10:17:04.798Z  

## 文件开头预览

```json
{
  "callId": "call-0491",
  "timestamp": "2026-09-24T10-17-03-908Z",
  "elapsed": 886,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【3】】【【4】】【【5】】【【7】】【【25】】【【26】】【【27】】【【34】】【【35】】【【67】】【【93】】【【197】】【【200】】【【263】】",
    "usage": {
      "prompt_tokens": 3104,
      "completion_tokens": 57,
      "total_tokens": 3161,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3104
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "7a7785ca-a96e-473a-8d31-d9aa0b7dc89b",
    "object": "chat.completion",
    "created": 1790245024,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【3】】【【4】】【【5】】【【7】】【【25】】【【26】】【【27】】【【34】】【【35】】【【67】】【【93】】【【197】】【【200】】【【263】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3104,
      "completion_tokens": 57,
      "total_tokens": 3161,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3104
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
