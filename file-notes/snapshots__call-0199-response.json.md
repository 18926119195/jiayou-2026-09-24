# call-0199-response.json

> **路径**: `snapshots\call-0199-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.5 KB  
> **最后修改**: 2026-09-24T10:15:48.088Z  

## 文件开头预览

```json
{
  "callId": "call-0199",
  "timestamp": "2026-09-24T10-15-47-233Z",
  "elapsed": 853,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【224】】【【225】】【【226】】【【227】】【【228】】【【229】】【【230】】【【232】】【【270】】【【271】】【【277】】【【302】】",
    "usage": {
      "prompt_tokens": 4032,
      "completion_tokens": 49,
      "total_tokens": 4081,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 4032
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "b1aa25f6-49af-47d7-9013-afcc558ef1b0",
    "object": "chat.completion",
    "created": 1790244947,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【224】】【【225】】【【226】】【【227】】【【228】】【【229】】【【230】】【【232】】【【270】】【【271】】【【277】】【【302】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 4032,
      "completion_tokens": 49,
      "total_tokens": 4081,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 4032
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
