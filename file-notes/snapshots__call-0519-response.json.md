# call-0519-response.json

> **路径**: `snapshots\call-0519-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.5 KB  
> **最后修改**: 2026-09-24T10:17:13.062Z  

## 文件开头预览

```json
{
  "callId": "call-0519",
  "timestamp": "2026-09-24T10-17-12-400Z",
  "elapsed": 661,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【325】】【【338】】【【330】】【【238】】【【239】】【【242】】【【243】】【【245】】【【246】】【【272】】【【279】】【【340】】【【337】】【【339】】",
    "usage": {
      "prompt_tokens": 3679,
      "completion_tokens": 57,
      "total_tokens": 3736,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3679
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "75126bb4-a079-41c0-a660-b6aceb3254d1",
    "object": "chat.completion",
    "created": 1790245032,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【325】】【【338】】【【330】】【【238】】【【239】】【【242】】【【243】】【【245】】【【246】】【【272】】【【279】】【【340】】【【337】】【【339】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3679,
      "completion_tokens": 57,
      "total_tokens": 3736,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3679
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
