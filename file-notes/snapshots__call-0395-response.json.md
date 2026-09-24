# call-0395-response.json

> **路径**: `snapshots\call-0395-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:16:37.325Z  

## 文件开头预览

```json
{
  "callId": "call-0395",
  "timestamp": "2026-09-24T10-16-36-660Z",
  "elapsed": 662,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【17】】【【36】】【【37】】【【46】】【【48】】【【54】】【【58】】【【100】】【【174】】",
    "usage": {
      "prompt_tokens": 3683,
      "completion_tokens": 37,
      "total_tokens": 3720,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3683
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "e8189e35-f759-4c70-8ce1-f333ceffa5fd",
    "object": "chat.completion",
    "created": 1790244996,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【17】】【【36】】【【37】】【【46】】【【48】】【【54】】【【58】】【【100】】【【174】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3683,
      "completion_tokens": 37,
      "total_tokens": 3720,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3683
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
