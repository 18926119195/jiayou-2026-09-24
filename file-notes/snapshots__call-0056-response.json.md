# call-0056-response.json

> **路径**: `snapshots\call-0056-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.5 KB  
> **最后修改**: 2026-09-24T10:58:35.679Z  

## 文件开头预览

```json
{
  "callId": "call-0056",
  "timestamp": "2026-09-24T10-58-35-028Z",
  "elapsed": 650,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【17】】【【18】】【【19】】【【30】】【【37】】【【47】】【【52】】【【90】】【【114】】【【152】】【【171】】【【204】】【【351】】",
    "usage": {
      "prompt_tokens": 3622,
      "completion_tokens": 53,
      "total_tokens": 3675,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3622
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "dadeb289-579d-47de-8b1c-61a6c44cdb5f",
    "object": "chat.completion",
    "created": 1790247515,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【17】】【【18】】【【19】】【【30】】【【37】】【【47】】【【52】】【【90】】【【114】】【【152】】【【171】】【【204】】【【351】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3622,
      "completion_tokens": 53,
      "total_tokens": 3675,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3622
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
