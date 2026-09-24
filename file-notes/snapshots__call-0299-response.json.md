# call-0299-response.json

> **路径**: `snapshots\call-0299-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:16:12.211Z  

## 文件开头预览

```json
{
  "callId": "call-0299",
  "timestamp": "2026-09-24T10-16-11-577Z",
  "elapsed": 632,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【102】】【【105】】【【181】】【【269】】【【363】】【【364】】【【365】】【【366】】",
    "usage": {
      "prompt_tokens": 3682,
      "completion_tokens": 33,
      "total_tokens": 3715,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3682
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "ba914b05-6bc0-4b45-a317-9d779d3dd3d4",
    "object": "chat.completion",
    "created": 1790244971,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【102】】【【105】】【【181】】【【269】】【【363】】【【364】】【【365】】【【366】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3682,
      "completion_tokens": 33,
      "total_tokens": 3715,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3682
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
