# call-0086-response.json

> **路径**: `snapshots\call-0086-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:58:37.973Z  

## 文件开头预览

```json
{
  "callId": "call-0086",
  "timestamp": "2026-09-24T10-58-37-435Z",
  "elapsed": 536,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【58】】【【69】】【【73】】【【93】】【【133】】【【238】】【【320】】",
    "usage": {
      "prompt_tokens": 3741,
      "completion_tokens": 29,
      "total_tokens": 3770,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3741
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "a3611db4-bb0c-4c84-81ab-bd41257fe764",
    "object": "chat.completion",
    "created": 1790247517,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【58】】【【69】】【【73】】【【93】】【【133】】【【238】】【【320】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3741,
      "completion_tokens": 29,
      "total_tokens": 3770,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3741
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
