# call-0202-response.json

> **路径**: `snapshots\call-0202-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.6 KB  
> **最后修改**: 2026-09-24T10:15:48.207Z  

## 文件开头预览

```json
{
  "callId": "call-0202",
  "timestamp": "2026-09-24T10-15-47-480Z",
  "elapsed": 725,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【12】】【【86】】【【87】】【【90】】【【117】】【【118】】【【119】】【【128】】【【137】】【【165】】【【177】】【【182】】【【231】】【【243】】【【317】】【【320】】",
    "usage": {
      "prompt_tokens": 3487,
      "completion_tokens": 65,
      "total_tokens": 3552,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3487
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "d54d80c6-ed31-4d64-9d7c-87e13195fda7",
    "object": "chat.completion",
    "created": 1790244947,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【12】】【【86】】【【87】】【【90】】【【117】】【【118】】【【119】】【【128】】【【137】】【【165】】【【177】】【【182】】【【231】】【【243】】【【317】】【【320】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3487,
      "completion_tokens": 65,
      "total_tokens": 3552,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3487
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
