# call-0037-response.json

> **路径**: `snapshots\call-0037-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T12:14:13.756Z  

## 文件开头预览

```json
{
  "callId": "call-0037",
  "timestamp": "2026-09-24T12-14-13-150Z",
  "elapsed": 606,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【58】】【【191】】【【220】】【【330】】【【331】】【【345】】",
    "usage": {
      "prompt_tokens": 3829,
      "completion_tokens": 25,
      "total_tokens": 3854,
      "prompt_tokens_details": {
        "cached_tokens": 3584
      },
      "prompt_cache_hit_tokens": 3584,
      "prompt_cache_miss_tokens": 245
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "4bbcac70-05a0-400e-b0a3-41a84d9c8aea",
    "object": "chat.completion",
    "created": 1790252053,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【58】】【【191】】【【220】】【【330】】【【331】】【【345】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3829,
      "completion_tokens": 25,
      "total_tokens": 3854,
      "prompt_tokens_details": {
        "cached_tokens": 3584
      },
      "prompt_cache_hit_tokens": 3584,
      "prompt_cache_miss_tokens": 245
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
