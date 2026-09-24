# call-0231-response.json

> **路径**: `snapshots\call-0231-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:15:57.638Z  

## 文件开头预览

```json
{
  "callId": "call-0231",
  "timestamp": "2026-09-24T10-15-57-082Z",
  "elapsed": 553,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【20】】【【123】】【【239】】【【319】】",
    "usage": {
      "prompt_tokens": 3765,
      "completion_tokens": 17,
      "total_tokens": 3782,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3765
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "25c9d53d-0fbf-4381-b905-dd04dbd7ad63",
    "object": "chat.completion",
    "created": 1790244957,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【20】】【【123】】【【239】】【【319】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3765,
      "completion_tokens": 17,
      "total_tokens": 3782,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3765
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
