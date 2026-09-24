# call-0413-response.json

> **路径**: `snapshots\call-0413-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.6 KB  
> **最后修改**: 2026-09-24T10:16:49.586Z  

## 文件开头预览

```json
{
  "callId": "call-0413",
  "timestamp": "2026-09-24T10-16-48-555Z",
  "elapsed": 1028,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【20】】【【35】】【【53】】【【57】】【【58】】【【71】】【【123】】【【126】】【【130】】【【135】】【【139】】【【149】】【【239】】【【248】】【【319】】",
    "usage": {
      "prompt_tokens": 3764,
      "completion_tokens": 61,
      "total_tokens": 3825,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3764
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "c3254b67-7cf8-4622-ba46-fa1256a33a7f",
    "object": "chat.completion",
    "created": 1790245008,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【20】】【【35】】【【53】】【【57】】【【58】】【【71】】【【123】】【【126】】【【130】】【【135】】【【139】】【【149】】【【239】】【【248】】【【319】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3764,
      "completion_tokens": 61,
      "total_tokens": 3825,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3764
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
