# call-0365-response.json

> **路径**: `snapshots\call-0365-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:16:34.935Z  

## 文件开头预览

```json
{
  "callId": "call-0365",
  "timestamp": "2026-09-24T10-16-34-083Z",
  "elapsed": 850,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【19】】【【28】】【【29】】【【62】】【【103】】【【122】】【【125】】【【166】】【【179】】【【199】】【【215】】",
    "usage": {
      "prompt_tokens": 3861,
      "completion_tokens": 45,
      "total_tokens": 3906,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3861
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "094868ae-4f27-4bce-a58e-de5aa4f8b329",
    "object": "chat.completion",
    "created": 1790244994,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【19】】【【28】】【【29】】【【62】】【【103】】【【122】】【【125】】【【166】】【【179】】【【199】】【【215】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3861,
      "completion_tokens": 45,
      "total_tokens": 3906,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3861
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
