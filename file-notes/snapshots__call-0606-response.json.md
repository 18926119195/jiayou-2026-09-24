# call-0606-response.json

> **路径**: `snapshots\call-0606-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:46.397Z  

## 文件开头预览

```json
{
  "callId": "call-0606",
  "timestamp": "2026-09-24T10-17-46-074Z",
  "elapsed": 321,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 4036,
      "completion_tokens": 2,
      "total_tokens": 4038,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 4036
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "6d489837-532c-4a24-9a60-d70b735d61fe",
    "object": "chat.completion",
    "created": 1790245066,
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
      "prompt_tokens": 4036,
      "completion_tokens": 2,
      "total_tokens": 4038,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 4036
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
