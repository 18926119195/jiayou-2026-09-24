# call-0423-response.json

> **路径**: `snapshots\call-0423-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:16:50.288Z  

## 文件开头预览

```json
{
  "callId": "call-0423",
  "timestamp": "2026-09-24T10-16-49-821Z",
  "elapsed": 463,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3942,
      "completion_tokens": 2,
      "total_tokens": 3944,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3942
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "d8cdbd57-f7c1-4a08-811c-d1d52677a95b",
    "object": "chat.completion",
    "created": 1790245010,
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
      "prompt_tokens": 3942,
      "completion_tokens": 2,
      "total_tokens": 3944,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3942
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
