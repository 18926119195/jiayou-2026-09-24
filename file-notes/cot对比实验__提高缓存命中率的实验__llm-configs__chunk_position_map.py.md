# chunk_position_map.py

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\chunk_position_map.py`  
> **分类**: 代码  
> **大小**: 3.5 KB  
> **最后修改**: 2026-09-24T11:04:29.285Z  

## 文件开头预览

```py
#!/usr/bin/env python3
# -*- coding: utf-8 -*-
import json
import re

with open('reasoning-output-Z1-Q4.json', 'r', encoding='utf-8') as f:
    data = json.load(f)

L23 = data['thinkingChain']
L24 = data['llmOutput']

print(f"L23 length: {len(L23)}")
print(f"L24 length: {len(L24)}")

# Chinese brackets
LB = '\u3010'  # 【
RB = '\u3011'  # 】

# Regex patterns
single_re = re.compile(re.escape(LB) + r'(\d+)' + re.escape(RB))
double_re = re.compile(re.escape(LB) + re.escape(LB) + r'(\d+)' + re.escape(RB) + re.escape(RB))

# Test
test = f'hello {LB}123{RB} world'
print(f"Test: matches={single_re.findall(test)}")

# Find all chunk mentions in L23
chunk_positions = {}  # chunk_id -> list of positions
for m in single_re.finditer(L23):
    cid = m.group(1)
    if cid not in chunk_positions:
        chunk_positions[cid] = []
    chunk_positions[cid].append(m.start())

print(f"Unique chunks mentioned in L23: {len(chunk_positions)}")
print(f"Chunks: {sorted(chunk_positions.keys(), key=int)}")

# Extract L24 paths
cn_nums = '\u4e00\u4e8c\u4e09\u56db\u4e94\u516d\u4e03\u516b\u4e5d\u5341'  # 一二三四五六七八九十
LU = '\u8def'  # 路
JING = '\u5f84'  # 径
path_re = re.compile(r'#\s*' + re.escape(LU) + re.escape(JING) + r'[' + cn_nums + r'][^#]*')

paths24 = []
for m in path_re.finditer(L24):
    block = m.group(0)
    nl = block.find('\n')
    title = block[:nl].strip() if nl > 0 else block[:80]
    chunks = list(set(double_re.findall(block)))
    paths24.append({'title': title, 'chunks': chunks, 'start': m.start()})
```
