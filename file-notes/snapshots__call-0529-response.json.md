# call-0529-response.json

> **路径**: `snapshots\call-0529-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:17:14.222Z  

## 文件开头预览

```json
{
  "callId": "call-0529",
  "timestamp": "2026-09-24T10-17-13-452Z",
  "elapsed": 767,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【26】】【【27】】【【89】】【【121】】【【122】】【【301】】",
    "usage": {
      "prompt_tokens": 3673,
      "completion_tokens": 25,
      "total_tokens": 3698,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3673
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "64d395a5-4529-4bee-ab2d-640b13a17134",
    "object": "chat.completion",
    "created": 1790245033,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【26】】【【27】】【【89】】【【121】】【【122】】【【301】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3673,
      "completion_tokens": 25,
      "total_tokens": 3698,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3673
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
