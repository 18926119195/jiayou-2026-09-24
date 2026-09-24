# call-0043-response.json

> **路径**: `snapshots\call-0043-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T12:14:14.216Z  

## 文件开头预览

```json
{
  "callId": "call-0043",
  "timestamp": "2026-09-24T12-14-13-622Z",
  "elapsed": 593,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 1066,
      "completion_tokens": 2,
      "total_tokens": 1068,
      "prompt_tokens_details": {
        "cached_tokens": 896
      },
      "prompt_cache_hit_tokens": 896,
      "prompt_cache_miss_tokens": 170
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "90e24b00-8ed9-46fd-abe2-3a4dda66c25a",
    "object": "chat.completion",
    "created": 1790252053,
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
      "prompt_tokens": 1066,
      "completion_tokens": 2,
      "total_tokens": 1068,
      "prompt_tokens_details": {
        "cached_tokens": 896
      },
      "prompt_cache_hit_tokens": 896,
      "prompt_cache_miss_tokens": 170
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
