# call-0012-response.json

> **路径**: `snapshots\call-0012-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T12:14:11.969Z  

## 文件开头预览

```json
{
  "callId": "call-0012",
  "timestamp": "2026-09-24T12-14-11-205Z",
  "elapsed": 763,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【214】】【【242】】【【216】】【【245】】【【57】】【【61】】【【62】】【【63】】【【126】】【【136】】【【74】】",
    "usage": {
      "prompt_tokens": 3732,
      "completion_tokens": 45,
      "total_tokens": 3777,
      "prompt_tokens_details": {
        "cached_tokens": 3584
      },
      "prompt_cache_hit_tokens": 3584,
      "prompt_cache_miss_tokens": 148
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "e7e8b91f-1557-478e-814b-df7e8e37fdd0",
    "object": "chat.completion",
    "created": 1790252051,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【214】】【【242】】【【216】】【【245】】【【57】】【【61】】【【62】】【【63】】【【126】】【【136】】【【74】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3732,
      "completion_tokens": 45,
      "total_tokens": 3777,
      "prompt_tokens_details": {
        "cached_tokens": 3584
      },
      "prompt_cache_hit_tokens": 3584,
      "prompt_cache_miss_tokens": 148
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
