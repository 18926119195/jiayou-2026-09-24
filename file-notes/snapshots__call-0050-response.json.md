# call-0050-response.json

> **路径**: `snapshots\call-0050-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:58:35.029Z  

## 文件开头预览

```json
{
  "callId": "call-0050",
  "timestamp": "2026-09-24T10-58-34-401Z",
  "elapsed": 625,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【4】】【【61】】【【266】】【【303】】【【316】】【【349】】【【350】】",
    "usage": {
      "prompt_tokens": 3682,
      "completion_tokens": 29,
      "total_tokens": 3711,
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
    "id": "0bb1012a-4ee8-4947-bbbe-3d9bad17d989",
    "object": "chat.completion",
    "created": 1790247514,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【4】】【【61】】【【266】】【【303】】【【316】】【【349】】【【350】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3682,
      "completion_tokens": 29,
      "total_tokens": 3711,
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
