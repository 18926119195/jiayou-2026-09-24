# call-0655-response.json

> **路径**: `snapshots\call-0655-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:17:58.891Z  

## 文件开头预览

```json
{
  "callId": "call-0655",
  "timestamp": "2026-09-24T10-17-58-189Z",
  "elapsed": 698,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3684,
      "completion_tokens": 2,
      "total_tokens": 3686,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3684
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "45a08f32-720b-4bb7-bbe7-adfa682b35be",
    "object": "chat.completion",
    "created": 1790245078,
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
      "prompt_tokens": 3684,
      "completion_tokens": 2,
      "total_tokens": 3686,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3684
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
