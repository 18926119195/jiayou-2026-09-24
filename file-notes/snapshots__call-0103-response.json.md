# call-0103-response.json

> **路径**: `snapshots\call-0103-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:58:47.252Z  

## 文件开头预览

```json
{
  "callId": "call-0103",
  "timestamp": "2026-09-24T10-58-46-440Z",
  "elapsed": 810,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【16】】【【46】】【【56】】【【62】】【【63】】【【126】】【【356】】",
    "usage": {
      "prompt_tokens": 3739,
      "completion_tokens": 29,
      "total_tokens": 3768,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3739
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "b9053057-eb9a-459d-a546-e422841e5da4",
    "object": "chat.completion",
    "created": 1790247527,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【16】】【【46】】【【56】】【【62】】【【63】】【【126】】【【356】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3739,
      "completion_tokens": 29,
      "total_tokens": 3768,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3739
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
