# call-0157-response.json

> **路径**: `snapshots\call-0157-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:59:01.399Z  

## 文件开头预览

```json
{
  "callId": "call-0157",
  "timestamp": "2026-09-24T10-59-00-620Z",
  "elapsed": 777,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【20】】【【25】】【【92】】【【93】】【【213】】【【217】】【【245】】【【247】】【【282】】【【295】】【【334】】",
    "usage": {
      "prompt_tokens": 3638,
      "completion_tokens": 45,
      "total_tokens": 3683,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3638
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "a963f7b9-b0ba-41f5-b520-8be9fa9f9f63",
    "object": "chat.completion",
    "created": 1790247540,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【20】】【【25】】【【92】】【【93】】【【213】】【【217】】【【245】】【【247】】【【282】】【【295】】【【334】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3638,
      "completion_tokens": 45,
      "total_tokens": 3683,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3638
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
