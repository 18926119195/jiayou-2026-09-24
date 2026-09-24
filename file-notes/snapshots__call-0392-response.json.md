# call-0392-response.json

> **路径**: `snapshots\call-0392-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:16:37.517Z  

## 文件开头预览

```json
{
  "callId": "call-0392",
  "timestamp": "2026-09-24T10-16-36-558Z",
  "elapsed": 956,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【181】】【【269】】【【363】】【【364】】【【365】】【【366】】",
    "usage": {
      "prompt_tokens": 3682,
      "completion_tokens": 25,
      "total_tokens": 3707,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3682
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "a0c81f9a-7cb0-417d-9e04-dfe4181a5969",
    "object": "chat.completion",
    "created": 1790244996,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【181】】【【269】】【【363】】【【364】】【【365】】【【366】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3682,
      "completion_tokens": 25,
      "total_tokens": 3707,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3682
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
