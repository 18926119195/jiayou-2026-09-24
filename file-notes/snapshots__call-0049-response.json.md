# call-0049-response.json

> **路径**: `snapshots\call-0049-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:58:34.983Z  

## 文件开头预览

```json
{
  "callId": "call-0049",
  "timestamp": "2026-09-24T10-58-34-400Z",
  "elapsed": 581,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【32】】【【47】】【【97】】【【104】】【【208】】【【285】】【【286】】",
    "usage": {
      "prompt_tokens": 3517,
      "completion_tokens": 29,
      "total_tokens": 3546,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3517
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "8e18de26-5b85-482b-97b7-02dac8d1991a",
    "object": "chat.completion",
    "created": 1790247514,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【32】】【【47】】【【97】】【【104】】【【208】】【【285】】【【286】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3517,
      "completion_tokens": 29,
      "total_tokens": 3546,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3517
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
