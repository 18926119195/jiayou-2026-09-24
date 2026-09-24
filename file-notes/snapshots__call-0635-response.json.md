# call-0635-response.json

> **路径**: `snapshots\call-0635-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:57.291Z  

## 文件开头预览

```json
{
  "callId": "call-0635",
  "timestamp": "2026-09-24T10-17-56-546Z",
  "elapsed": 741,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3856,
      "completion_tokens": 2,
      "total_tokens": 3858,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3856
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "cb9a9544-2a96-41ad-94c6-25948a3e6331",
    "object": "chat.completion",
    "created": 1790245076,
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
      "prompt_tokens": 3856,
      "completion_tokens": 2,
      "total_tokens": 3858,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3856
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
