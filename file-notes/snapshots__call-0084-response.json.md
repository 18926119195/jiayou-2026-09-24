# call-0084-response.json

> **路径**: `snapshots\call-0084-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:58:37.775Z  

## 文件开头预览

```json
{
  "callId": "call-0084",
  "timestamp": "2026-09-24T10-58-37-181Z",
  "elapsed": 592,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【92】】【【215】】【【47】】【【49】】【【52】】【【202】】【【157】】【【256】】",
    "usage": {
      "prompt_tokens": 3507,
      "completion_tokens": 33,
      "total_tokens": 3540,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3507
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "ffd82af1-0b39-40a7-8f35-6cf035c4481a",
    "object": "chat.completion",
    "created": 1790247517,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【92】】【【215】】【【47】】【【49】】【【52】】【【202】】【【157】】【【256】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3507,
      "completion_tokens": 33,
      "total_tokens": 3540,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3507
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
