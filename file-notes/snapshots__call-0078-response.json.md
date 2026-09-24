# call-0078-response.json

> **路径**: `snapshots\call-0078-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:58:37.410Z  

## 文件开头预览

```json
{
  "callId": "call-0078",
  "timestamp": "2026-09-24T10-58-36-791Z",
  "elapsed": 617,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【95】】【【250】】【【284】】【【299】】",
    "usage": {
      "prompt_tokens": 3657,
      "completion_tokens": 17,
      "total_tokens": 3674,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3657
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "03db637e-391e-4ee3-8741-c11a24c3136a",
    "object": "chat.completion",
    "created": 1790247517,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【95】】【【250】】【【284】】【【299】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3657,
      "completion_tokens": 17,
      "total_tokens": 3674,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3657
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
