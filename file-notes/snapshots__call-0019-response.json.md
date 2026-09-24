# call-0019-response.json

> **路径**: `snapshots\call-0019-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T12:14:12.463Z  

## 文件开头预览

```json
{
  "callId": "call-0019",
  "timestamp": "2026-09-24T12-14-11-870Z",
  "elapsed": 592,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【88】】【【276】】",
    "usage": {
      "prompt_tokens": 3638,
      "completion_tokens": 9,
      "total_tokens": 3647,
      "prompt_tokens_details": {
        "cached_tokens": 3456
      },
      "prompt_cache_hit_tokens": 3456,
      "prompt_cache_miss_tokens": 182
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "f2b10cc5-8732-46e7-9f83-50279e3e9172",
    "object": "chat.completion",
    "created": 1790252052,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【88】】【【276】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3638,
      "completion_tokens": 9,
      "total_tokens": 3647,
      "prompt_tokens_details": {
        "cached_tokens": 3456
      },
      "prompt_cache_hit_tokens": 3456,
      "prompt_cache_miss_tokens": 182
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
