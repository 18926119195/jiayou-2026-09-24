# call-0419-response.json

> **路径**: `snapshots\call-0419-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:16:50.342Z  

## 文件开头预览

```json
{
  "callId": "call-0419",
  "timestamp": "2026-09-24T10-16-49-454Z",
  "elapsed": 884,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【17】】【【37】】【【64】】【【74】】【【289】】【【306】】",
    "usage": {
      "prompt_tokens": 3455,
      "completion_tokens": 25,
      "total_tokens": 3480,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3455
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "e0535198-204f-468f-a5e0-7a5b6ec2e3cc",
    "object": "chat.completion",
    "created": 1790245009,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【17】】【【37】】【【64】】【【74】】【【289】】【【306】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3455,
      "completion_tokens": 25,
      "total_tokens": 3480,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3455
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
