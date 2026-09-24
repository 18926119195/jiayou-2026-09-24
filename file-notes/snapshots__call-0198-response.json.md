# call-0198-response.json

> **路径**: `snapshots\call-0198-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:15:47.770Z  

## 文件开头预览

```json
{
  "callId": "call-0198",
  "timestamp": "2026-09-24T10-15-47-211Z",
  "elapsed": 557,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【13】】【【14】】【【46】】【【47】】【【67】】【【311】】",
    "usage": {
      "prompt_tokens": 3988,
      "completion_tokens": 25,
      "total_tokens": 4013,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3988
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "6e8d44b0-7aa2-4f3f-afc1-33fb731fd99c",
    "object": "chat.completion",
    "created": 1790244947,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【13】】【【14】】【【46】】【【47】】【【67】】【【311】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3988,
      "completion_tokens": 25,
      "total_tokens": 4013,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3988
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
