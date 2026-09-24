# call-0064-response.json

> **路径**: `snapshots\call-0064-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:58:36.267Z  

## 文件开头预览

```json
{
  "callId": "call-0064",
  "timestamp": "2026-09-24T10-58-35-678Z",
  "elapsed": 586,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3592,
      "completion_tokens": 2,
      "total_tokens": 3594,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3592
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "bbd63f24-0608-46fd-898d-3d10250a0415",
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
      "prompt_tokens": 3592,
      "completion_tokens": 2,
      "total_tokens": 3594,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3592
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
