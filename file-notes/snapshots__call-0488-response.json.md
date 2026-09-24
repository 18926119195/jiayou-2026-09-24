# call-0488-response.json

> **路径**: `snapshots\call-0488-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:17:03.954Z  

## 文件开头预览

```json
{
  "callId": "call-0488",
  "timestamp": "2026-09-24T10-17-03-510Z",
  "elapsed": 441,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【14】】【【250】】",
    "usage": {
      "prompt_tokens": 3413,
      "completion_tokens": 9,
      "total_tokens": 3422,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3413
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "f5d084a1-dc94-4079-868e-280cad024416",
    "object": "chat.completion",
    "created": 1790245023,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【14】】【【250】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3413,
      "completion_tokens": 9,
      "total_tokens": 3422,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3413
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
