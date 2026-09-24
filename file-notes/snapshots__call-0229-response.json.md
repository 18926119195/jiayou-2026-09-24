# call-0229-response.json

> **路径**: `snapshots\call-0229-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:15:57.424Z  

## 文件开头预览

```json
{
  "callId": "call-0229",
  "timestamp": "2026-09-24T10-15-57-080Z",
  "elapsed": 340,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【273】】【【336】】【【437】】",
    "usage": {
      "prompt_tokens": 3955,
      "completion_tokens": 13,
      "total_tokens": 3968,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3955
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "32cb413e-756e-4bf0-ba97-f2f9515f4ac7",
    "object": "chat.completion",
    "created": 1790244957,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【273】】【【336】】【【437】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3955,
      "completion_tokens": 13,
      "total_tokens": 3968,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3955
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
