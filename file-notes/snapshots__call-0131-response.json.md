# call-0131-response.json

> **路径**: `snapshots\call-0131-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:58:50.081Z  

## 文件开头预览

```json
{
  "callId": "call-0131",
  "timestamp": "2026-09-24T10-58-49-386Z",
  "elapsed": 692,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【58】】【【65】】【【111】】【【133】】【【149】】【【242】】【【340】】【【353】】【【356】】",
    "usage": {
      "prompt_tokens": 3748,
      "completion_tokens": 37,
      "total_tokens": 3785,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3748
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "88dc052b-aecd-4424-bd66-987443a329b5",
    "object": "chat.completion",
    "created": 1790247529,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【58】】【【65】】【【111】】【【133】】【【149】】【【242】】【【340】】【【353】】【【356】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3748,
      "completion_tokens": 37,
      "total_tokens": 3785,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3748
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
