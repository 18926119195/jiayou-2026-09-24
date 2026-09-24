# call-0254-response.json

> **路径**: `snapshots\call-0254-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:16:00.085Z  

## 文件开头预览

```json
{
  "callId": "call-0254",
  "timestamp": "2026-09-24T10-15-59-349Z",
  "elapsed": 732,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【50】】【【55】】",
    "usage": {
      "prompt_tokens": 3736,
      "completion_tokens": 9,
      "total_tokens": 3745,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3736
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "cf6e290f-b73c-48dd-ae5c-e1793edb69ef",
    "object": "chat.completion",
    "created": 1790244959,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【50】】【【55】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3736,
      "completion_tokens": 9,
      "total_tokens": 3745,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3736
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
