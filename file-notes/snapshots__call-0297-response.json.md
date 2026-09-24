# call-0297-response.json

> **路径**: `snapshots\call-0297-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:16:12.068Z  

## 文件开头预览

```json
{
  "callId": "call-0297",
  "timestamp": "2026-09-24T10-16-11-410Z",
  "elapsed": 656,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【15】】【【43】】【【45】】【【85】】【【126】】【【275】】【【290】】",
    "usage": {
      "prompt_tokens": 3661,
      "completion_tokens": 29,
      "total_tokens": 3690,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3661
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "b64bcb6e-b0bc-4c3d-8583-d88192050591",
    "object": "chat.completion",
    "created": 1790244971,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【15】】【【43】】【【45】】【【85】】【【126】】【【275】】【【290】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3661,
      "completion_tokens": 29,
      "total_tokens": 3690,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3661
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
