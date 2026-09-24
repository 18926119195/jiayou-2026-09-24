# call-0583-response.json

> **路径**: `snapshots\call-0583-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:17:37.913Z  

## 文件开头预览

```json
{
  "callId": "call-0583",
  "timestamp": "2026-09-24T10-17-37-432Z",
  "elapsed": 478,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【17】】【【161】】",
    "usage": {
      "prompt_tokens": 1683,
      "completion_tokens": 9,
      "total_tokens": 1692,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 1683
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "baf63585-07fd-48e6-8098-ff9478fce600",
    "object": "chat.completion",
    "created": 1790245057,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【17】】【【161】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 1683,
      "completion_tokens": 9,
      "total_tokens": 1692,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 1683
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
