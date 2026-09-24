# call-0369-response.json

> **路径**: `snapshots\call-0369-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:16:35.241Z  

## 文件开头预览

```json
{
  "callId": "call-0369",
  "timestamp": "2026-09-24T10-16-34-705Z",
  "elapsed": 533,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【3】】【【293】】",
    "usage": {
      "prompt_tokens": 3788,
      "completion_tokens": 9,
      "total_tokens": 3797,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3788
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "434465d2-d10b-4101-b9aa-53f58a2bfde8",
    "object": "chat.completion",
    "created": 1790244994,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【3】】【【293】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3788,
      "completion_tokens": 9,
      "total_tokens": 3797,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3788
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
