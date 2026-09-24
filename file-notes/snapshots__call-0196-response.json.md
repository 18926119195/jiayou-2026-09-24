# call-0196-response.json

> **路径**: `snapshots\call-0196-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:15:47.551Z  

## 文件开头预览

```json
{
  "callId": "call-0196",
  "timestamp": "2026-09-24T10-15-46-982Z",
  "elapsed": 566,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3945,
      "completion_tokens": 2,
      "total_tokens": 3947,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3945
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "f9335683-d483-4e88-8433-63b965e10f98",
    "object": "chat.completion",
    "created": 1790244947,
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
      "prompt_tokens": 3945,
      "completion_tokens": 2,
      "total_tokens": 3947,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3945
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
