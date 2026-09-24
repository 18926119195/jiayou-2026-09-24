# call-0532-response.json

> **路径**: `snapshots\call-0532-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:17:14.537Z  

## 文件开头预览

```json
{
  "callId": "call-0532",
  "timestamp": "2026-09-24T10-17-13-768Z",
  "elapsed": 767,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【13】】【【29】】【【37】】【【114】】【【135】】【【136】】【【144】】【【153】】【【187】】",
    "usage": {
      "prompt_tokens": 3411,
      "completion_tokens": 37,
      "total_tokens": 3448,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3411
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "643b2610-602a-43b2-ad47-a4f312700a64",
    "object": "chat.completion",
    "created": 1790245033,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【13】】【【29】】【【37】】【【114】】【【135】】【【136】】【【144】】【【153】】【【187】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3411,
      "completion_tokens": 37,
      "total_tokens": 3448,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3411
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
