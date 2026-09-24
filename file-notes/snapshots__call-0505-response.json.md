# call-0505-response.json

> **路径**: `snapshots\call-0505-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:17:11.946Z  

## 文件开头预览

```json
{
  "callId": "call-0505",
  "timestamp": "2026-09-24T10-17-10-991Z",
  "elapsed": 953,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【121】】",
    "usage": {
      "prompt_tokens": 3611,
      "completion_tokens": 5,
      "total_tokens": 3616,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3611
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "e7e067ec-4a19-468c-b38b-5fc87d559c40",
    "object": "chat.completion",
    "created": 1790245031,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【121】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3611,
      "completion_tokens": 5,
      "total_tokens": 3616,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3611
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
