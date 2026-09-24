# call-0065-response.json

> **路径**: `snapshots\call-0065-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:58:36.254Z  

## 文件开头预览

```json
{
  "callId": "call-0065",
  "timestamp": "2026-09-24T10-58-35-736Z",
  "elapsed": 516,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【88】】【【276】】",
    "usage": {
      "prompt_tokens": 3638,
      "completion_tokens": 9,
      "total_tokens": 3647,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3638
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "4f25982d-ef2e-4964-85fb-042580355a63",
    "object": "chat.completion",
    "created": 1790247515,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【88】】【【276】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3638,
      "completion_tokens": 9,
      "total_tokens": 3647,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3638
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
