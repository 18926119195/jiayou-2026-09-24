# call-0073-response.json

> **路径**: `snapshots\call-0073-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:58:36.922Z  

## 文件开头预览

```json
{
  "callId": "call-0073",
  "timestamp": "2026-09-24T10-58-36-342Z",
  "elapsed": 579,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【2】】【【10】】【【18】】【【37】】【【44】】【【56】】【【80】】【【99】】【【154】】",
    "usage": {
      "prompt_tokens": 3519,
      "completion_tokens": 37,
      "total_tokens": 3556,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3519
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "dd98c191-7877-4792-9793-9d1e8897837a",
    "object": "chat.completion",
    "created": 1790247516,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【2】】【【10】】【【18】】【【37】】【【44】】【【56】】【【80】】【【99】】【【154】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3519,
      "completion_tokens": 37,
      "total_tokens": 3556,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3519
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
