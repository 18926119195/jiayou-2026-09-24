# runner-stdout.log

> **路径**: `问题一\runs\2026-09-24-cache-test-rerun\logs\runner-stdout.log`  
> **分类**: 文本输出  
> **大小**: 427.5 KB  
> **最后修改**: 2026-09-24T11:47:58.167Z  

## 文件开头预览

```log
[init] SRC_DIR = C:\Users\Administrator\Desktop\chenggong-jiachi-master\完整的运作
[init] RUN_DIR = C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-24-cache-test-rerun
[init] LOG_DIR = C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-24-cache-test-rerun\logs
[init] SNAPSHOT_DIR = C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-24-cache-test-rerun\snapshots
[init] FINAL_DIR = C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-24-cache-test-rerun\final
[init] docuverse = C:\Users\Administrator\Desktop\chenggong-jiachi-master\docuverse_cartographies_squizoanalythiques_Fe_lix_Guattari_1789114122714.docuverse.json
[init] env vars:
  OUTPUT_PATH = C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-24-cache-test-rerun\noun-recall-results.json
  RECALL_RESULTS_PATH = C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-24-cache-test-rerun\noun-recall-results.json
  CANDIDATE_TEXTS_PATH = C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-24-cache-test-rerun\candidate-texts-for-llm.json
  TRACEBACK_MAP_PATH = C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-24-cache-test-rerun\material-traceback-map.json
  LLM_SNAPSHOT_DIR = C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-24-cache-test-rerun\snapshots
  LLM_CONCURRENCY = 8
  DOCUVERSE_PATH = C:\Users\Administrator\Desktop\chenggong-jiachi-master\docuverse_cartographies_squizoanalythiques_Fe_lix_Guattari_1789114122714.docuverse.json
  NOUN_INDEX_PATH = C:\Users\Administrator\Desktop\chenggong-jiachi-master\完整的运作\final-noun-index.json
  QUESTIONS_PATH = C:\Users\Administrator\Desktop\chenggong-jiachi-master\完整的运作\test-questions.json
[init] 15 questions to run: Z1-Q1, Z1-Q2, Z1-Q3, Z1-Q4, Z2-Q1, Z2-Q2, Z2-Q3, Z2-Q4, Z3-Q1, Z3-Q2, Z3-Q3, Z4-Q1, Z4-Q2, Z4-Q3, Z4-Q4
[llmClient] 快照根目录: C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-24-cache-test-rerun\snapshots
LLM: https://api.deepseek.com model=deepseek-flash thinking=disabled
加载数据...
  chunk 数: 1446（无全局拼接）
  名词数（原始）: 16244, 问题数: 15
  ⚠️ FILTER_BLACKLIST=1 但黑名单文件不存在: C:\Users\Administrator\Desktop\chenggong-jiachi-master\完整的运作\noun-blacklist.json（跳过过滤）
========== 拓扑链召回引擎（两步架构）==========
全量名词: 16244, 问题数: 1
Token预算分批: 最多2500 tokens/批次, 并发: 8, 拓扑窗口: 2 名词, 分数阈值: 80


--- [Z1-Q1] Pierre Janet和Freud对无意识的观点有何不同？ ---
[llmClient] [Z1-Q1] 全新子目录，从 call-0001 开始编号

[call-0001] LLM 调用开始...
  QuestionId: Z1-Q1
  子目录: C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-24-cache-test-rerun\snapshots\Z1-Q1
  Prompt 长度: 8283 字符
  Max tokens: 32768
  重试策略: 最多 3 次（仅网络错误/5xx/408/429）

[call-0002] LLM 调用开始...
  QuestionId: Z1-Q1
  子目录: C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-24-cache-test-rerun\snapshots\Z1-Q1
  Prompt 长度: 8285 字符
  Max tokens: 32768
  重试策略: 最多 3 次（仅网络错误/5xx/408/429）

[call-0003] LLM 调用开始...
  QuestionId: Z1-Q1
  子目录: C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-24-cache-test-rerun\snapshots\Z1-Q1
  Prompt 长度: 8331 字符
  Max tokens: 32768
```
