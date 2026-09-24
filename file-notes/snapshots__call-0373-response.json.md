# call-0373-response.json

> **路径**: `snapshots\call-0373-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:16:35.448Z  

## 文件开头预览

```json
{
  "callId": "call-0373",
  "timestamp": "2026-09-24T10-16-34-823Z",
  "elapsed": 623,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【114】】【【147】】【【154】】【【169】】【【282】】",
    "usage": {
      "prompt_tokens": 3737,
      "completion_tokens": 21,
      "total_tokens": 3758,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3737
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "1cdddd82-11c9-4c7a-8a64-ca2283c74dba",
    "object": "chat.completion",
    "created": 1790244995,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【114】】【【147】】【【154】】【【169】】【【282】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3737,
      "completion_tokens": 21,
      "total_tokens": 3758,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3737
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
