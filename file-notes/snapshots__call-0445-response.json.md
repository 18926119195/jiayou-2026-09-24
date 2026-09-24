# call-0445-response.json

> **路径**: `snapshots\call-0445-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:16:52.399Z  

## 文件开头预览

```json
{
  "callId": "call-0445",
  "timestamp": "2026-09-24T10-16-51-745Z",
  "elapsed": 650,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【42】】【【63】】【【209】】【【210】】【【213】】【【241】】【【267】】【【273】】",
    "usage": {
      "prompt_tokens": 3270,
      "completion_tokens": 33,
      "total_tokens": 3303,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3270
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "dd80abb5-08c9-4cf2-82ff-5a0c51aa65c6",
    "object": "chat.completion",
    "created": 1790245011,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【42】】【【63】】【【209】】【【210】】【【213】】【【241】】【【267】】【【273】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3270,
      "completion_tokens": 33,
      "total_tokens": 3303,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3270
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
