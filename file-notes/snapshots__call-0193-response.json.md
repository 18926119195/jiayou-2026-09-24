# call-0193-response.json

> **路径**: `snapshots\call-0193-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:15:47.397Z  

## 文件开头预览

```json
{
  "callId": "call-0193",
  "timestamp": "2026-09-24T10-15-46-736Z",
  "elapsed": 659,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【31】】【【86】】【【121】】【【133】】【【177】】",
    "usage": {
      "prompt_tokens": 3347,
      "completion_tokens": 21,
      "total_tokens": 3368,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3347
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "dd0759cb-7edd-455c-bdb7-52d9703a60e7",
    "object": "chat.completion",
    "created": 1790244946,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【31】】【【86】】【【121】】【【133】】【【177】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3347,
      "completion_tokens": 21,
      "total_tokens": 3368,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3347
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
