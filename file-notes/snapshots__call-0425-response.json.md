# call-0425-response.json

> **路径**: `snapshots\call-0425-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:16:50.617Z  

## 文件开头预览

```json
{
  "callId": "call-0425",
  "timestamp": "2026-09-24T10-16-49-882Z",
  "elapsed": 731,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【5】】【【13】】【【14】】【【65】】【【67】】【【99】】【【251】】【【311】】【【325】】【【380】】",
    "usage": {
      "prompt_tokens": 3985,
      "completion_tokens": 41,
      "total_tokens": 4026,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3985
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "c0d45d2a-3b0c-4406-8069-6d52ed7690f3",
    "object": "chat.completion",
    "created": 1790245010,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【5】】【【13】】【【14】】【【65】】【【67】】【【99】】【【251】】【【311】】【【325】】【【380】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3985,
      "completion_tokens": 41,
      "total_tokens": 4026,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3985
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
