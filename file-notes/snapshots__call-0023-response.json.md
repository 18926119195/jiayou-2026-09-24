# call-0023-response.json

> **路径**: `snapshots\call-0023-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T12:14:12.350Z  

## 文件开头预览

```json
{
  "callId": "call-0023",
  "timestamp": "2026-09-24T12-14-11-969Z",
  "elapsed": 380,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3475,
      "completion_tokens": 2,
      "total_tokens": 3477,
      "prompt_tokens_details": {
        "cached_tokens": 3328
      },
      "prompt_cache_hit_tokens": 3328,
      "prompt_cache_miss_tokens": 147
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "339b0018-b6ce-48aa-b230-9dda7915cffc",
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
      "prompt_tokens": 3475,
      "completion_tokens": 2,
      "total_tokens": 3477,
      "prompt_tokens_details": {
        "cached_tokens": 3328
      },
      "prompt_cache_hit_tokens": 3328,
      "prompt_cache_miss_tokens": 147
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
