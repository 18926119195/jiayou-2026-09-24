# call-0022-response.json

> **路径**: `snapshots\call-0022-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T12:14:12.683Z  

## 文件开头预览

```json
{
  "callId": "call-0022",
  "timestamp": "2026-09-24T12-14-11-945Z",
  "elapsed": 737,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3493,
      "completion_tokens": 2,
      "total_tokens": 3495,
      "prompt_tokens_details": {
        "cached_tokens": 3328
      },
      "prompt_cache_hit_tokens": 3328,
      "prompt_cache_miss_tokens": 165
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "df55b1e6-6979-4861-a95b-3f02eb203c21",
    "object": "chat.completion",
    "created": 1790252052,
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
      "prompt_tokens": 3493,
      "completion_tokens": 2,
      "total_tokens": 3495,
      "prompt_tokens_details": {
        "cached_tokens": 3328
      },
      "prompt_cache_hit_tokens": 3328,
      "prompt_cache_miss_tokens": 165
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
