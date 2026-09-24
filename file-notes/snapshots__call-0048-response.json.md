# call-0048-response.json

> **路径**: `snapshots\call-0048-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:58:35.124Z  

## 文件开头预览

```json
{
  "callId": "call-0048",
  "timestamp": "2026-09-24T10-58-34-400Z",
  "elapsed": 722,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【52】】【【21】】【【86】】【【229】】【【279】】【【290】】【【350】】",
    "usage": {
      "prompt_tokens": 3605,
      "completion_tokens": 29,
      "total_tokens": 3634,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3605
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "58f2b4bb-a110-4838-a057-dcd871169585",
    "object": "chat.completion",
    "created": 1790247514,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【52】】【【21】】【【86】】【【229】】【【279】】【【290】】【【350】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3605,
      "completion_tokens": 29,
      "total_tokens": 3634,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3605
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
