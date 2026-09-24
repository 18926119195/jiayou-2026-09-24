# call-0503-response.json

> **路径**: `snapshots\call-0503-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:17:11.825Z  

## 文件开头预览

```json
{
  "callId": "call-0503",
  "timestamp": "2026-09-24T10-17-10-976Z",
  "elapsed": 848,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【83】】【【259】】【【320】】【【333】】",
    "usage": {
      "prompt_tokens": 3778,
      "completion_tokens": 17,
      "total_tokens": 3795,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3778
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "a078221d-c18a-4a6c-8292-725007547610",
    "object": "chat.completion",
    "created": 1790245031,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【83】】【【259】】【【320】】【【333】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3778,
      "completion_tokens": 17,
      "total_tokens": 3795,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3778
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
