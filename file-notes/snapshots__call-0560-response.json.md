# call-0560-response.json

> **路径**: `snapshots\call-0560-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.3 KB  
> **最后修改**: 2026-09-24T10:17:36.178Z  

## 文件开头预览

```json
{
  "callId": "call-0560",
  "timestamp": "2026-09-24T10-17-35-487Z",
  "elapsed": 688,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【13】】【【14】】【【201】】【【311】】【【325】】【【380】】",
    "usage": {
      "prompt_tokens": 3988,
      "completion_tokens": 25,
      "total_tokens": 4013,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3988
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "21770efb-356d-42a2-866d-e64e1ca090f8",
    "object": "chat.completion",
    "created": 1790245055,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【13】】【【14】】【【201】】【【311】】【【325】】【【380】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3988,
      "completion_tokens": 25,
      "total_tokens": 4013,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3988
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
