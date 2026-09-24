# reorder-prompts-for-cache.py

> **路径**: `cot对比实验\提高缓存命中率的实验\reorder-prompts-for-cache.py`  
> **分类**: 代码  
> **大小**: 3.4 KB  
> **最后修改**: 2026-09-24T06:24:25.412Z  

## 文件开头预览

```py
"""
提升缓存命中率实验：将 15 个全量 prompt 中的"问题头+要求+格式+规范+策略"
全部移到末尾、把"全量材料"区块挪到最前面。

约束：字字不差，仅换位置（用 find 找到【【全量材料】】的字节位置，按字节切两段、再反向拼接）。

缓存原理：
  DeepSeek API 的 prefix cache 命中是从 prompt 开头算起的连续相同前缀。
  原顺序：[问题头 + 1446 chunks]   → 每个问题开头不同，cache 命中率=0%
  新顺序：[1446 chunks + 问题头]   → 1446 chunks 部分在 15 个问题间完全一致，
                                     第二个问题开始就能命中前面 165k tokens 的前缀
"""

import os
import re

SCRIPT_DIR = os.path.dirname(os.path.abspath(__file__))
SRC_DIR = os.path.dirname(SCRIPT_DIR)  # 父目录 cot对比实验/
OUT_DIR = SCRIPT_DIR

MARKER = '【【全量材料】】'

QIDS = [
    'Z1-Q1', 'Z1-Q2', 'Z1-Q3', 'Z1-Q4',
    'Z2-Q1', 'Z2-Q2', 'Z2-Q3', 'Z2-Q4',
    'Z3-Q1', 'Z3-Q2', 'Z3-Q3',
    'Z4-Q1', 'Z4-Q2', 'Z4-Q3', 'Z4-Q4',
]

total_src_bytes = 0
total_out_bytes = 0

for qid in QIDS:
    src_path = os.path.join(SRC_DIR, f'multipath-prompt-cot-{qid}.txt')
    out_path = os.path.join(OUT_DIR, f'multipath-prompt-cot-{qid}.txt')

    with open(src_path, 'r', encoding='utf-8') as f:
        src = f.read()

    idx = src.find(MARKER)
    if idx == -1:
        print(f'❌ {qid}: 未找到 {MARKER}，已跳过')
        continue

    # 在 marker 位置切两段：[0, idx) + [idx, end)，然后反向拼接
    header_part = src[:idx]
    chunks_part = src[idx:]
    swapped = chunks_part + header_part

    with open(out_path, 'w', encoding='utf-8') as f:
```
