# call-0463-response.json

> **路径**: `snapshots\call-0463-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:17:02.095Z  

## 文件开头预览

```json
{
  "callId": "call-0463",
  "timestamp": "2026-09-24T10-17-01-240Z",
  "elapsed": 851,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【102】】【【137】】【【140】】【【149】】【【169】】【【174】】【【282】】【【301】】",
    "usage": {
      "prompt_tokens": 3729,
      "completion_tokens": 33,
      "total_tokens": 3762,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3729
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "b79263c1-ba88-4a49-a984-a55994580bc9",
    "object": "chat.completion",
    "created": 1790245021,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【102】】【【137】】【【140】】【【149】】【【169】】【【174】】【【282】】【【301】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3729,
      "completion_tokens": 33,
      "total_tokens": 3762,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3729
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
