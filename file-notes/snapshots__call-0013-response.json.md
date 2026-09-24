# call-0013-response.json

> **路径**: `snapshots\call-0013-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T12:14:11.681Z  

## 文件开头预览

```json
{
  "callId": "call-0013",
  "timestamp": "2026-09-24T12-14-11-260Z",
  "elapsed": 420,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3811,
      "completion_tokens": 2,
      "total_tokens": 3813,
      "prompt_tokens_details": {
        "cached_tokens": 3584
      },
      "prompt_cache_hit_tokens": 3584,
      "prompt_cache_miss_tokens": 227
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "e05e4603-0bdc-42e6-90d4-f46f40ec6cc4",
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
      "prompt_tokens": 3811,
      "completion_tokens": 2,
      "total_tokens": 3813,
      "prompt_tokens_details": {
        "cached_tokens": 3584
      },
      "prompt_cache_hit_tokens": 3584,
      "prompt_cache_miss_tokens": 227
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
