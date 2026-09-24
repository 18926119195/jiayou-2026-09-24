# call-0485-response.json

> **路径**: `snapshots\call-0485-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:17:04.196Z  

## 文件开头预览

```json
{
  "callId": "call-0485",
  "timestamp": "2026-09-24T10-17-03-435Z",
  "elapsed": 758,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【28】】【【35】】【【46】】【【100】】【【347】】【【364】】",
    "usage": {
      "prompt_tokens": 3675,
      "completion_tokens": 25,
      "total_tokens": 3700,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3675
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "407da4eb-ca9d-4105-8dc4-2cfaf93c8cad",
    "object": "chat.completion",
    "created": 1790245023,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【28】】【【35】】【【46】】【【100】】【【347】】【【364】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3675,
      "completion_tokens": 25,
      "total_tokens": 3700,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3675
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
