# call-0412-response.json

> **路径**: `snapshots\call-0412-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:16:49.456Z  

## 文件开头预览

```json
{
  "callId": "call-0412",
  "timestamp": "2026-09-24T10-16-48-554Z",
  "elapsed": 899,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【4】】【【23】】【【51】】【【54】】【【118】】【【203】】【【204】】【【205】】【【340】】",
    "usage": {
      "prompt_tokens": 3786,
      "completion_tokens": 37,
      "total_tokens": 3823,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3786
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "21a9c630-7f38-446b-9578-d7f9d1be4fd0",
    "object": "chat.completion",
    "created": 1790245008,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【4】】【【23】】【【51】】【【54】】【【118】】【【203】】【【204】】【【205】】【【340】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3786,
      "completion_tokens": 37,
      "total_tokens": 3823,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3786
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
