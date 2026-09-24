# call-0614-response.json

> **路径**: `snapshots\call-0614-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:47.388Z  

## 文件开头预览

```json
{
  "callId": "call-0614",
  "timestamp": "2026-09-24T10-17-46-741Z",
  "elapsed": 645,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3857,
      "completion_tokens": 2,
      "total_tokens": 3859,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3857
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "d154bb2f-b5d6-4b92-a5df-19a3d33cc552",
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
      "prompt_tokens": 3857,
      "completion_tokens": 2,
      "total_tokens": 3859,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3857
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
