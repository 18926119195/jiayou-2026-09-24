# call-0444-response.json

> **路径**: `snapshots\call-0444-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:16:52.472Z  

## 文件开头预览

```json
{
  "callId": "call-0444",
  "timestamp": "2026-09-24T10-16-51-732Z",
  "elapsed": 737,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【103】】【【119】】【【120】】【【160】】【【161】】【【203】】【【276】】【【290】】【【313】】【【314】】【【315】】",
    "usage": {
      "prompt_tokens": 3483,
      "completion_tokens": 45,
      "total_tokens": 3528,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3483
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "160e4f85-8dc5-4729-bd50-8f8d13456dbf",
    "object": "chat.completion",
    "created": 1790245012,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【103】】【【119】】【【120】】【【160】】【【161】】【【203】】【【276】】【【290】】【【313】】【【314】】【【315】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3483,
      "completion_tokens": 45,
      "total_tokens": 3528,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3483
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
