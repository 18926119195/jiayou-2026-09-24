# call-0306-response.json

> **路径**: `snapshots\call-0306-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:16:12.779Z  

## 文件开头预览

```json
{
  "callId": "call-0306",
  "timestamp": "2026-09-24T10-16-12-211Z",
  "elapsed": 567,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【12】】【【13】】【【115】】【【119】】【【120】】【【121】】【【160】】【【189】】【【276】】【【290】】【【313】】",
    "usage": {
      "prompt_tokens": 3491,
      "completion_tokens": 45,
      "total_tokens": 3536,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3491
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "21dcfec9-410c-4cb5-8c56-11a4f914a438",
    "object": "chat.completion",
    "created": 1790244972,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【12】】【【13】】【【115】】【【119】】【【120】】【【121】】【【160】】【【189】】【【276】】【【290】】【【313】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3491,
      "completion_tokens": 45,
      "total_tokens": 3536,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3491
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
