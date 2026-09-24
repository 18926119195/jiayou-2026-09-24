# call-0319-response.json

> **路径**: `snapshots\call-0319-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:16:23.160Z  

## 文件开头预览

```json
{
  "callId": "call-0319",
  "timestamp": "2026-09-24T10-16-22-574Z",
  "elapsed": 584,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【32】】【【37】】【【66】】【【83】】【【139】】【【216】】【【223】】【【224】】【【229】】【【258】】【【385】】",
    "usage": {
      "prompt_tokens": 3955,
      "completion_tokens": 45,
      "total_tokens": 4000,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3955
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "f7b0d890-5967-4157-ab7e-66a4aa52b6c4",
    "object": "chat.completion",
    "created": 1790244982,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【32】】【【37】】【【66】】【【83】】【【139】】【【216】】【【223】】【【224】】【【229】】【【258】】【【385】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3955,
      "completion_tokens": 45,
      "total_tokens": 4000,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3955
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
