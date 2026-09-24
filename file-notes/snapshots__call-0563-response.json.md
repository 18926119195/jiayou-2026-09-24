# call-0563-response.json

> **路径**: `snapshots\call-0563-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:17:36.932Z  

## 文件开头预览

```json
{
  "callId": "call-0563",
  "timestamp": "2026-09-24T10-17-35-848Z",
  "elapsed": 1082,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【92】】【【251】】【【286】】【【287】】【【291】】【【294】】【【138】】【【276】】【【139】】【【91】】【【6】】",
    "usage": {
      "prompt_tokens": 3483,
      "completion_tokens": 45,
      "total_tokens": 3528,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3483
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "b25297a7-29ce-48d3-a686-19df967a2b65",
    "object": "chat.completion",
    "created": 1790245056,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【92】】【【251】】【【286】】【【287】】【【291】】【【294】】【【138】】【【276】】【【139】】【【91】】【【6】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3483,
      "completion_tokens": 45,
      "total_tokens": 3528,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3483
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
