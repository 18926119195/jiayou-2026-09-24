# call-0612-response.json

> **路径**: `snapshots\call-0612-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:17:47.035Z  

## 文件开头预览

```json
{
  "callId": "call-0612",
  "timestamp": "2026-09-24T10-17-46-635Z",
  "elapsed": 397,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【163】】【【248】】【【286】】",
    "usage": {
      "prompt_tokens": 3260,
      "completion_tokens": 13,
      "total_tokens": 3273,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3260
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "18ec5ace-1c6a-4429-821c-eadc65733b5a",
    "object": "chat.completion",
    "created": 1790245066,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【163】】【【248】】【【286】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3260,
      "completion_tokens": 13,
      "total_tokens": 3273,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3260
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
