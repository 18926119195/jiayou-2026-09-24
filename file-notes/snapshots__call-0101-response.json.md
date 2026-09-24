# call-0101-response.json

> **路径**: `snapshots\call-0101-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.8 KB  
> **最后修改**: 2026-09-24T10:58:47.032Z  

## 文件开头预览

```json
{
  "callId": "call-0101",
  "timestamp": "2026-09-24T10-58-46-406Z",
  "elapsed": 625,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【7】】【【17】】【【18】】【【19】】【【30】】【【37】】【【46】】【【47】】【【52】】【【105】】【【106】】【【108】】【【114】】【【152】】【【171】】【【181】】【【203】】【【204】】【【213】】【【286】】【【294】】【【351】】【【361】】",
    "usage": {
      "prompt_tokens": 3629,
      "completion_tokens": 93,
      "total_tokens": 3722,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3629
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "498308bf-82af-45aa-8896-7721b880f246",
    "object": "chat.completion",
    "created": 1790247526,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【7】】【【17】】【【18】】【【19】】【【30】】【【37】】【【46】】【【47】】【【52】】【【105】】【【106】】【【108】】【【114】】【【152】】【【171】】【【181】】【【203】】【【204】】【【213】】【【286】】【【294】】【【351】】【【361】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3629,
      "completion_tokens": 93,
      "total_tokens": 3722,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3629
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
