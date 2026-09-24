# call-0490-response.json

> **路径**: `snapshots\call-0490-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:17:04.412Z  

## 文件开头预览

```json
{
  "callId": "call-0490",
  "timestamp": "2026-09-24T10-17-03-619Z",
  "elapsed": 790,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【42】】【【43】】【【44】】【【52】】【【63】】【【209】】【【210】】【【213】】【【267】】",
    "usage": {
      "prompt_tokens": 3270,
      "completion_tokens": 37,
      "total_tokens": 3307,
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
    "id": "4bef803a-eceb-46ab-8c1c-df45ae667f22",
    "object": "chat.completion",
    "created": 1790245023,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【42】】【【43】】【【44】】【【52】】【【63】】【【209】】【【210】】【【213】】【【267】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3270,
      "completion_tokens": 37,
      "total_tokens": 3307,
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
