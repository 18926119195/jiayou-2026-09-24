# README.txt

> **路径**: `问题一\runs\2026-09-24-cache-test-rerun\README.txt`  
> **分类**: 文本输出  
> **大小**: 2.4 KB  
> **最后修改**: 2026-09-24T11:43:10.109Z  

## 文件开头预览

```txt
# 2026-09-24 Cache Test Rerun - 15 题全量复跑

## 实验说明

复刻 `runs/2026-09-23-cache-test-rerun-remainder` 的生产流程，全量重跑 15 道题（Z1-Q1 ~ Z4-Q4，Z3-Q4 在 test-questions.json 里不存在故跳过）。`2026-09-23-cache-test-rerun-remainder` 目录的数据**完全不动**。

## 数据保存策略

- `_before-backup/`：跑前备份 `完整的运作/` 全部文件（5 json + 15 multipath-prompt + 15 reasoning-output，共 34 个文件）
- `snapshots/`：15 题 LLM 调用快照（逐题子目录）
- `logs/`：各步骤日志和汇总报告（`pipeline.log` + `rerun-<QID>.log` + `rerun-summary.txt`）
- `final/`：跑完后 15 题最终输出副本（3 json + 15 prompt + 15 reasoning）
- 顶层目录：`noun-recall-results.json` + `candidate-texts-for-llm.json` + `material-traceback-map.json` + 15 prompt + 15 reasoning

## 核心策略（不变）

在 `完整的运作/recall-nouns-llm.js` 的 for 循环前已经标注：
- 题间顺序执行（for 循环）：最大化 prompt-cache 命中率
- 题内 8 批次并发：保持召回效率

代码逻辑本身不变，只让策略注释与实际行为对齐。

## 缓存命中率预期

跨题 noun list 共享前缀 → 第 2 题开始命中率高（参考上次结果 88-99.9%）。

## 各步骤耗时估算

| 步骤 | 耗时 |
|------|------|
| recall-nouns-llm（15题，串行） | ~3 分钟 |
| build-prompt-with-traceback（×15） | ~1 分钟 |
| generate-multipath-prompt（×15） | ~15 秒 |
| run-reasoning（×15，LLM推理） | ~45-75 分钟 |
| **合计** | **约 50-80 分钟** |

## 文件清单

### 跑前备份（_before-backup/）
- `noun-recall-results.json` / `candidate-texts-for-llm.json` / `material-traceback-map.json` / `final-noun-index.json`
- `multipath-prompt-Z{x}-Q{y}.txt` × 15
- `reasoning-output-Z{x}-Q{y}.json` × 15

### 跑时快照（snapshots/）
- `Z{x}-Q{y}/call-NNNN-request.json` + `call-NNNN-response.json` + `call-NNNN-prompt.txt` + `call-NNNN-output.txt`

### 跑后副本（final/）
- 3 个 json（noun-recall / candidate-texts / material-traceback-map）
- 15 个 multipath-prompt
- 15 个 reasoning-output
```
