# call-0378-response.json

> **路径**: `snapshots\call-0378-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:16:35.989Z  

## 文件开头预览

```json
{
  "callId": "call-0378",
  "timestamp": "2026-09-24T10-16-35-446Z",
  "elapsed": 540,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【367】】【【368】】【【369】】【【370】】",
    "usage": {
      "prompt_tokens": 3950,
      "completion_tokens": 17,
      "total_tokens": 3967,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3950
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "334764d3-9109-45c3-b2af-8b1597fa57ac",
    "object": "chat.completion",
    "created": 1790244995,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【367】】【【368】】【【369】】【【370】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3950,
      "completion_tokens": 17,
      "total_tokens": 3967,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3950
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
