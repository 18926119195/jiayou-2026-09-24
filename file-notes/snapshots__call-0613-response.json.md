# call-0613-response.json

> **路径**: `snapshots\call-0613-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:17:47.281Z  

## 文件开头预览

```json
{
  "callId": "call-0613",
  "timestamp": "2026-09-24T10-17-46-675Z",
  "elapsed": 604,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【2】】【【76】】【【214】】【【296】】【【297】】【【315】】",
    "usage": {
      "prompt_tokens": 3538,
      "completion_tokens": 25,
      "total_tokens": 3563,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3538
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "40b2716b-16a6-480d-bf2c-f7fe655cc2d5",
    "object": "chat.completion",
    "created": 1790245066,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【2】】【【76】】【【214】】【【296】】【【297】】【【315】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3538,
      "completion_tokens": 25,
      "total_tokens": 3563,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3538
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
