# call-0059-response.json

> **路径**: `snapshots\call-0059-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:58:35.737Z  

## 文件开头预览

```json
{
  "callId": "call-0059",
  "timestamp": "2026-09-24T10-58-35-150Z",
  "elapsed": 585,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3811,
      "completion_tokens": 2,
      "total_tokens": 3813,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3811
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "8a02c956-b058-4203-abcd-f4297096d88d",
    "object": "chat.completion",
    "created": 1790247515,
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
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3811
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
