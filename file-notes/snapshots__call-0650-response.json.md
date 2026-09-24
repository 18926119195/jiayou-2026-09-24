# call-0650-response.json

> **路径**: `snapshots\call-0650-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:58.475Z  

## 文件开头预览

```json
{
  "callId": "call-0650",
  "timestamp": "2026-09-24T10-17-57-721Z",
  "elapsed": 751,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3988,
      "completion_tokens": 2,
      "total_tokens": 3990,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3988
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "1598f956-6a9d-40a9-bd9c-d27743aaa44d",
    "object": "chat.completion",
    "created": 1790245077,
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
      "prompt_tokens": 3988,
      "completion_tokens": 2,
      "total_tokens": 3990,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3988
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
