# call-0296-response.json

> **路径**: `snapshots\call-0296-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:16:11.855Z  

## 文件开头预览

```json
{
  "callId": "call-0296",
  "timestamp": "2026-09-24T10-16-11-377Z",
  "elapsed": 477,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3858,
      "completion_tokens": 2,
      "total_tokens": 3860,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3858
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "bba01a2f-16fe-4c0c-a3aa-1a7ab1eae45d",
    "object": "chat.completion",
    "created": 1790244971,
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
      "prompt_tokens": 3858,
      "completion_tokens": 2,
      "total_tokens": 3860,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3858
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
