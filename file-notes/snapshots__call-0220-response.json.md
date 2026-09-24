# call-0220-response.json

> **路径**: `snapshots\call-0220-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:15:49.530Z  

## 文件开头预览

```json
{
  "callId": "call-0220",
  "timestamp": "2026-09-24T10-15-49-019Z",
  "elapsed": 508,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【1】】【【3】】【【21】】【【42】】【【76】】【【81】】【【106】】【【107】】【【128】】【【174】】【【211】】",
    "usage": {
      "prompt_tokens": 3166,
      "completion_tokens": 45,
      "total_tokens": 3211,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3166
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "0a678bae-7aa6-45b8-9e57-b21eec46af51",
    "object": "chat.completion",
    "created": 1790244949,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【1】】【【3】】【【21】】【【42】】【【76】】【【81】】【【106】】【【107】】【【128】】【【174】】【【211】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3166,
      "completion_tokens": 45,
      "total_tokens": 3211,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3166
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
