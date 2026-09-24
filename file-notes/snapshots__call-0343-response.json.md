# call-0343-response.json

> **路径**: `snapshots\call-0343-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:16:25.993Z  

## 文件开头预览

```json
{
  "callId": "call-0343",
  "timestamp": "2026-09-24T10-16-25-432Z",
  "elapsed": 559,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【15】】【【43】】【【45】】【【85】】【【126】】【【269】】【【275】】【【320】】【【321】】【【322】】",
    "usage": {
      "prompt_tokens": 3654,
      "completion_tokens": 41,
      "total_tokens": 3695,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3654
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "7482cb92-dc18-4273-a842-7983f7e2c706",
    "object": "chat.completion",
    "created": 1790244985,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【15】】【【43】】【【45】】【【85】】【【126】】【【269】】【【275】】【【320】】【【321】】【【322】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3654,
      "completion_tokens": 41,
      "total_tokens": 3695,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3654
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
