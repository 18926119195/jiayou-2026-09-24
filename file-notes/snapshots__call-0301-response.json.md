# call-0301-response.json

> **路径**: `snapshots\call-0301-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:16:12.403Z  

## 文件开头预览

```json
{
  "callId": "call-0301",
  "timestamp": "2026-09-24T10-16-11-696Z",
  "elapsed": 706,
  "success": true,
  "retries": [],
  "response": {
    "text": "NONE",
    "usage": {
      "prompt_tokens": 3867,
      "completion_tokens": 2,
      "total_tokens": 3869,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3867
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "e2e7f8fc-02be-48e9-b293-dbd9acf3f1c5",
    "object": "chat.completion",
    "created": 1790244972,
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
      "prompt_tokens": 3867,
      "completion_tokens": 2,
      "total_tokens": 3869,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3867
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
