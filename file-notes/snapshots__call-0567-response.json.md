# call-0567-response.json

> **路径**: `snapshots\call-0567-response.json`  
> **分类**: 配置 / 数据  
> **大小**: 1.6 KB  
> **最后修改**: 2026-09-24T10:17:36.758Z  

## 文件开头预览

```json
{
  "callId": "call-0567",
  "timestamp": "2026-09-24T10-17-36-089Z",
  "elapsed": 666,
  "success": true,
  "retries": [],
  "response": {
    "text": "【【8】】【【10】】【【11】】【【12】】【【55】】【【63】】【【73】】【【85】】【【145】】【【155】】【【163】】【【166】】【【223】】【【229】】【【259】】【【275】】",
    "usage": {
      "prompt_tokens": 3256,
      "completion_tokens": 65,
      "total_tokens": 3321,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3256
    },
    "truncated": false,
    "finishReason": "stop"
  },
  "rawResponse": {
    "id": "7b26cbca-f527-4f18-a120-c0107181a098",
    "object": "chat.completion",
    "created": 1790245056,
    "model": "deepseek-flash",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "【【8】】【【10】】【【11】】【【12】】【【55】】【【63】】【【73】】【【85】】【【145】】【【155】】【【163】】【【166】】【【223】】【【229】】【【259】】【【275】】"
        },
        "logprobs": null,
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 3256,
      "completion_tokens": 65,
      "total_tokens": 3321,
      "prompt_tokens_details": {
        "cached_tokens": 0
      },
      "prompt_cache_hit_tokens": 0,
      "prompt_cache_miss_tokens": 3256
    },
    "system_fingerprint": "aeb56401ca74e127821c4f9126dcb669"
  }
}
```
