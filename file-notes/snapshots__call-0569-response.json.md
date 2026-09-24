# call-0569-response.json

> **路径**: `snapshots\call-0569-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.5 KB  
> **最后修改**: 2026-09-24T10:17:36.824Z  

## 文件开头预览

```json
{
  "callId": "call-0569",
  "timestamp": "2026-09-24T10-17-36-273Z",
  "elapsed": 549,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【210】】【【242】】【【311】】【【310】】【【377】】【【143】】【【279】】【【234】】【【249】】【【248】】【【41】】【【106】】【【90】】",
    "usage": {
      "prompt_tokens": 3853,
      "completion_tokens": 53,
      "total_tokens": 3906,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3853
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "5218b1f4-66ee-49c1-9442-8556fcd07380",
    "object": "chat.completion",
    "created": 1790245056,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【210】】【【242】】【【311】】【【310】】【【377】】【【143】】【【279】】【【234】】【【249】】【【248】】【【41】】【【106】】【【90】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3853,
      "completion_tokens": 53,
      "total_tokens": 3906,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3853
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
