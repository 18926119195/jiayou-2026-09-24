# call-0605-response.json

> **路径**: `snapshots\call-0605-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:17:46.636Z  

## 文件开头预览

```json
{
  "callId": "call-0605",
  "timestamp": "2026-09-24T10-17-46-054Z",
  "elapsed": 580,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【140】】【【142】】【【175】】【【311】】【【13】】【【14】】",
    "usage": {
      "prompt_tokens": 3992,
      "completion_tokens": 25,
      "total_tokens": 4017,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3992
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "1341d01a-1680-42e0-a27b-3946f1ad6449",
    "object": "chat.completion",
    "created": 1790245066,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【140】】【【142】】【【175】】【【311】】【【13】】【【14】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3992,
      "completion_tokens": 25,
      "total_tokens": 4017,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3992
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
