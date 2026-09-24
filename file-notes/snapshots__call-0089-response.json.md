# call-0089-response.json

> **路径**: `snapshots\call-0089-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:58:38.508Z  

## 文件开头预览

```json
{
  "callId": "call-0089",
  "timestamp": "2026-09-24T10-58-37-721Z",
  "elapsed": 785,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 1066,
      "completion_tokens": 2,
      "total_tokens": 1068,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 1066
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "441d6e0d-fa23-4791-aa6f-819cfa63b690",
    "object": "chat.completion",
    "created": 1790247517,
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
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 1066
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
