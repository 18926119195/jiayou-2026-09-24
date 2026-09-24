# call-0466-response.json

> **路径**: `snapshots\call-0466-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:17:01.991Z  

## 文件开头预览

```json
{
  "callId": "call-0466",
  "timestamp": "2026-09-24T10-17-01-413Z",
  "elapsed": 575,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【34】】【【60】】【【255】】【【261】】【【265】】",
    "usage": {
      "prompt_tokens": 3800,
      "completion_tokens": 21,
      "total_tokens": 3821,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3800
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "7342306a-528a-4f0b-810c-e612792040d0",
    "object": "chat.completion",
    "created": 1790245021,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【34】】【【60】】【【255】】【【261】】【【265】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3800,
      "completion_tokens": 21,
      "total_tokens": 3821,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3800
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
