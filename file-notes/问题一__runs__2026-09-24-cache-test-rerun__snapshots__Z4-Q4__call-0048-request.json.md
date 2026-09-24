# call-0048-request.json

> **路径**: `问题一\runs\2026-09-24-cache-test-rerun\snapshots\Z4-Q4\call-0048-request.json`  
> **分类**: 配置 / 数据  
> **大小**: 2.3 KB  
> **最后修改**: 2026-09-24T11:47:55.069Z  

## 文件开头预览

```json
{
  "callId": "call-0048",
  "questionId": "Z4-Q4",
  "timestamp": "2026-09-24T11-47-55-067Z",
  "promptLength": 649,
  "promptPreview": "问题：根据本文档，拉康派的临床技术手册在哪里可以下载？\n\n材料：\n\n【【1】】(命中: 0)\ndonnées • des savoirs et des techniques de l'époque\n\n【【2】】(命中: 0)\nune pénétration générale\n\n【【3】】(命中: 0)\nœuvre par les micro-proces-\n\n【【4】】(命中: 0)\n- des techniques de sémiotisation économique, par exemple\n\n【【5】】(命中: 0)\nidéologies qui pretendaient, naguère, servir de guide pour reconstruire la société sur des bases\n\n---\n\n要求：输出2-4条独立推理路径，每条路径包含多个步骤，每步可引用一个或多个材料【【N】】。\n\n格式：\n\n# 路径一：[标题]\n\n步骤1：使用【【X】】，提取...\n步骤2：综合【【Y】】【【Z】】，对比...\n\n结论：[此路径结论]\n\n（继续路径二、三...）\n...",
  "fullPrompt": "问题：根据本文档，拉康派的临床技术手册在哪里可以下载？\n\n材料：\n\n【【1】】(命中: 0)\ndonnées • des savoirs et des techniques de l'époque\n\n【【2】】(命中: 0)\nune pénétration générale\n\n【【3】】(命中: 0)\nœuvre par les micro-proces-\n\n【【4】】(命中: 0)\n- des techniques de sémiotisation économique, par exemple\n\n【【5】】(命中: 0)\nidéologies qui pretendaient, naguère, servir de guide pour reconstruire la société sur des bases\n\n---\n\n要求：输出2-4条独立推理路径，每条路径包含多个步骤，每步可引用一个或多个材料【【N】】。\n\n格式：\n\n# 路径一：[标题]\n\n步骤1：使用【【X】】，提取...\n步骤2：综合【【Y】】【【Z】】，对比...\n\n结论：[此路径结论]\n\n（继续路径二、三...）\n\n**引用规范**：\n- 单个材料：使用【【N】】，提取...，判断...\n- 多个材料：综合【【N】】【【M】】，对比/交叉验证/综合提取...\n\n**推理策略**：\n- 对比论证：对比不同材料中的矛盾或差异\n- 交叉验证：从多个材料中找到互相支撑的证据\n- 综合支撑：从多处提取一致的特征或模式",
  "options": {
    "maxTokens": 32768
  },
  "retryPolicy": {
    "maxAttempts": 3,
    "baseDelayMs": 1000,
    "maxDelayMs": 10000
  }
}
```
