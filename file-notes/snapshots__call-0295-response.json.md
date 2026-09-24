# call-0295-response.json

> **路径**: `snapshots\call-0295-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T10:16:11.696Z  

## 文件开头预览

```json
{
  "callId": "call-0295",
  "timestamp": "2026-09-24T10-16-11-157Z",
  "elapsed": 538,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【2】】",
    "usage": {
      "prompt_tokens": 3539,
      "completion_tokens": 5,
      "total_tokens": 3544,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3539
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "47be1738-e83f-44a0-9353-64a6ad65cfe9",
    "object": "chat.completion",
    "created": 1790244971,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【2】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3539,
      "completion_tokens": 5,
      "total_tokens": 3544,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3539
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
