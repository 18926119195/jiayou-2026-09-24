# call-0092-response.json

> **路径**: `snapshots\call-0092-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.7 KB  
> **最后修改**: 2026-09-24T10:58:46.560Z  

## 文件开头预览

```json
{
  "callId": "call-0092",
  "timestamp": "2026-09-24T10-58-45-814Z",
  "elapsed": 743,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【8】】【【17】】【【20】】【【26】】【【27】】【【34】】【【149】】【【175】】【【176】】【【204】】【【220】】【【232】】【【234】】【【242】】【【254】】【【256】】【【284】】【【289】】【【295】】【【316】】",
    "usage": {
      "prompt_tokens": 3664,
      "completion_tokens": 81,
      "total_tokens": 3745,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3664
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "dc8e7379-1bc6-43fd-8e3a-3cb9a24a3594",
    "object": "chat.completion",
    "created": 1790247526,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【8】】【【17】】【【20】】【【26】】【【27】】【【34】】【【149】】【【175】】【【176】】【【204】】【【220】】【【232】】【【234】】【【242】】【【254】】【【256】】【【284】】【【289】】【【295】】【【316】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3664,
      "completion_tokens": 81,
      "total_tokens": 3745,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3664
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
