# call-0440-response.json

> **路径**: `snapshots\call-0440-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:16:52.404Z  

## 文件开头预览

```json
{
  "callId": "call-0440",
  "timestamp": "2026-09-24T10-16-51-321Z",
  "elapsed": 1079,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【23】】【【35】】【【36】】【【37】】【【46】】【【58】】【【100】】【【124】】【【321】】",
    "usage": {
      "prompt_tokens": 3675,
      "completion_tokens": 37,
      "total_tokens": 3712,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3675
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "95ccc494-579d-42d3-97be-e1e091be845e",
    "object": "chat.completion",
    "created": 1790245011,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【23】】【【35】】【【36】】【【37】】【【46】】【【58】】【【100】】【【124】】【【321】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3675,
      "completion_tokens": 37,
      "total_tokens": 3712,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3675
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
