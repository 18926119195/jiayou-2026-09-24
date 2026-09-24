# call-0495-response.json

> **路径**: `snapshots\call-0495-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.5 KB  
> **最后修改**: 2026-09-24T10:17:11.063Z  

## 文件开头预览

```json
{
  "callId": "call-0495",
  "timestamp": "2026-09-24T10-17-10-389Z",
  "elapsed": 673,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【6】】【【79】】【【80】】【【98】】【【114】】【【122】】【【129】】【【141】】【【201】】【【235】】【【268】】【【474】】",
    "usage": {
      "prompt_tokens": 4152,
      "completion_tokens": 49,
      "total_tokens": 4201,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 4152
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "0eec1cae-3eb0-46f3-b1eb-e18c22f12df4",
    "object": "chat.completion",
    "created": 1790245030,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【6】】【【79】】【【80】】【【98】】【【114】】【【122】】【【129】】【【141】】【【201】】【【235】】【【268】】【【474】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 4152,
      "completion_tokens": 49,
      "total_tokens": 4201,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 4152
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
