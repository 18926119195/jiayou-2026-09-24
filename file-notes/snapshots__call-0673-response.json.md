# call-0673-response.json

> **路径**: `snapshots\call-0673-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:18:00.053Z  

## 文件开头预览

```json
{
  "callId": "call-0673",
  "timestamp": "2026-09-24T10-17-59-342Z",
  "elapsed": 709,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 1683,
      "completion_tokens": 2,
      "total_tokens": 1685,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 1683
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "01f20fca-50e3-407a-b1b8-3478bec406e1",
    "object": "chat.completion",
    "created": 1790245079,
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
      "prompt_tokens": 1683,
      "completion_tokens": 2,
      "total_tokens": 1685,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 1683
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
