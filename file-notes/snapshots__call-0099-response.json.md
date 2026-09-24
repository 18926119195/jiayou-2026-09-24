# call-0099-response.json

> **路径**: `snapshots\call-0099-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:58:46.441Z  

## 文件开头预览

```json
{
  "callId": "call-0099",
  "timestamp": "2026-09-24T10-58-45-819Z",
  "elapsed": 621,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【29】】【【30】】【【36】】【【146】】【【162】】【【163】】【【164】】【【175】】",
    "usage": {
      "prompt_tokens": 3567,
      "completion_tokens": 33,
      "total_tokens": 3600,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3567
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "e9625af2-0368-4236-b7bc-28a4991af54d",
    "object": "chat.completion",
    "created": 1790247526,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【29】】【【30】】【【36】】【【146】】【【162】】【【163】】【【164】】【【175】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3567,
      "completion_tokens": 33,
      "total_tokens": 3600,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3567
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
