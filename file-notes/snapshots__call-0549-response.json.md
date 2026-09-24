# call-0549-response.json

> **路径**: `snapshots\call-0549-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:17:35.360Z  

## 文件开头预览

```json
{
  "callId": "call-0549",
  "timestamp": "2026-09-24T10-17-34-532Z",
  "elapsed": 825,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【247】】【【255】】【【256】】【【293】】【【335】】",
    "usage": {
      "prompt_tokens": 3783,
      "completion_tokens": 21,
      "total_tokens": 3804,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3783
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "81aae298-ed32-4607-bea8-5a9495e1e1e5",
    "object": "chat.completion",
    "created": 1790245054,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【247】】【【255】】【【256】】【【293】】【【335】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3783,
      "completion_tokens": 21,
      "total_tokens": 3804,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3783
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
