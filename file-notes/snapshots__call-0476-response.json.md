# call-0476-response.json

> **路径**: `snapshots\call-0476-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:17:03.318Z  

## 文件开头预览

```json
{
  "callId": "call-0476",
  "timestamp": "2026-09-24T10-17-02-482Z",
  "elapsed": 832,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【43】】【【151】】【【227】】【【244】】【【245】】【【285】】【【304】】【【305】】",
    "usage": {
      "prompt_tokens": 3279,
      "completion_tokens": 33,
      "total_tokens": 3312,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3279
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "21e57f00-3f6a-4e0f-bb1f-4338dda16aaa",
    "object": "chat.completion",
    "created": 1790245022,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【43】】【【151】】【【227】】【【244】】【【245】】【【285】】【【304】】【【305】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3279,
      "completion_tokens": 33,
      "total_tokens": 3312,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3279
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
