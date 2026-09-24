# call-0587-response.json

> **路径**: `snapshots\call-0587-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:17:45.155Z  

## 文件开头预览

```json
{
  "callId": "call-0587",
  "timestamp": "2026-09-24T10-17-44-592Z",
  "elapsed": 560,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【1】】【【22】】【【24】】【【58】】【【139】】【【186】】【【194】】【【195】】【【204】】【【259】】",
    "usage": {
      "prompt_tokens": 4066,
      "completion_tokens": 41,
      "total_tokens": 4107,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 4066
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "c50dad15-6c51-48e4-bfd9-1f6c30383e03",
    "object": "chat.completion",
    "created": 1790245064,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【1】】【【22】】【【24】】【【58】】【【139】】【【186】】【【194】】【【195】】【【204】】【【259】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 4066,
      "completion_tokens": 41,
      "total_tokens": 4107,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 4066
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
