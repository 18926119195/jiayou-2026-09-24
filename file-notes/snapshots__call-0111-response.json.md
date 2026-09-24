# call-0111-response.json

> **路径**: `snapshots\call-0111-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:58:47.686Z  

## 文件开头预览

```json
{
  "callId": "call-0111",
  "timestamp": "2026-09-24T10-58-47-204Z",
  "elapsed": 481,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【17】】【【45】】【【272】】【【279】】",
    "usage": {
      "prompt_tokens": 3772,
      "completion_tokens": 17,
      "total_tokens": 3789,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3772
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "45d5c230-789b-46f8-9a91-9a95bd94d735",
    "object": "chat.completion",
    "created": 1790247527,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【17】】【【45】】【【272】】【【279】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3772,
      "completion_tokens": 17,
      "total_tokens": 3789,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3772
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
