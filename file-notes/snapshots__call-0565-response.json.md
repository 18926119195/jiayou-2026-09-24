# call-0565-response.json

> **路径**: `snapshots\call-0565-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:17:36.667Z  

## 文件开头预览

```json
{
  "callId": "call-0565",
  "timestamp": "2026-09-24T10-17-35-973Z",
  "elapsed": 692,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【120】】【【196】】【【247】】【【252】】【【253】】【【279】】【【287】】【【325】】【【338】】【【340】】",
    "usage": {
      "prompt_tokens": 3684,
      "completion_tokens": 41,
      "total_tokens": 3725,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3684
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "6c31be63-0dc7-4dda-8979-a8e20e6e50f0",
    "object": "chat.completion",
    "created": 1790245056,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【120】】【【196】】【【247】】【【252】】【【253】】【【279】】【【287】】【【325】】【【338】】【【340】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3684,
      "completion_tokens": 41,
      "total_tokens": 3725,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3684
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
