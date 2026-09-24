# call-0330-response.json

> **路径**: `snapshots\call-0330-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:16:24.539Z  

## 文件开头预览

```json
{
  "callId": "call-0330",
  "timestamp": "2026-09-24T10-16-24-012Z",
  "elapsed": 524,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【5】】【【14】】【【15】】【【51】】【【128】】【【179】】【【181】】【【193】】【【259】】【【340】】",
    "usage": {
      "prompt_tokens": 3794,
      "completion_tokens": 41,
      "total_tokens": 3835,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3794
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "ab93c028-ddf4-4037-a5ac-d2c5a0eef3ce",
    "object": "chat.completion",
    "created": 1790244984,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【5】】【【14】】【【15】】【【51】】【【128】】【【179】】【【181】】【【193】】【【259】】【【340】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3794,
      "completion_tokens": 41,
      "total_tokens": 3835,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3794
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
