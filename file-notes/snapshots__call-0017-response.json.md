# call-0017-response.json

> **路径**: `snapshots\call-0017-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T12:14:12.103Z  

## 文件开头预览

```json
{
  "callId": "call-0017",
  "timestamp": "2026-09-24T12-14-11-681Z",
  "elapsed": 421,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3631,
      "completion_tokens": 2,
      "total_tokens": 3633,
      "prompt_tokens_details": {
        "cached_tokens": 3456
      },
      "prompt_cache_hit_tokens": 3456,
      "prompt_cache_miss_tokens": 175
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "ed99abb5-a335-46e9-8161-8ac7e683d0ad",
    "object": "chat.completion",
    "created": 1790252051,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "NONE"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3631,
      "completion_tokens": 2,
      "total_tokens": 3633,
      "prompt_tokens_details": {
        "cached_tokens": 3456
      },
      "prompt_cache_hit_tokens": 3456,
      "prompt_cache_miss_tokens": 175
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
