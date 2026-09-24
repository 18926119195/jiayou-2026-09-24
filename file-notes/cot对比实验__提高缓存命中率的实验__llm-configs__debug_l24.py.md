# debug_l24.py

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\debug_l24.py`  
> **分类**: 代码  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:14:58.906Z  

## 文件开头预览

```py
# -*- coding: utf-8 -*-
import json
import re

lines = []
with open('reasoning-output-Z1-Q3.json', 'r', encoding='utf-8') as f:
    data = json.load(f)

line24 = data[23]
line23 = data[22]

lines.append(f'L23 length: {len(line23)}')
lines.append(f'L24 length: {len(line24)}')
lines.append(f'L24 first 200 chars repr: {repr(line24[:200])}')

# Test simple regex
hits = re.findall(r'#\s*路径[一二三四五六七八九十]', line24)
lines.append(f'simple regex hits: {len(hits)} -> {hits}')

# Test the full regex
pat = re.compile(r'#\s*路径([一二三四五六七八九十]+)[：:](.+?)(?=\n---+|\n#|\Z)', re.DOTALL)
matches = list(pat.finditer(line24))
lines.append(f'full regex matches: {len(matches)}')
for m in matches[:10]:
    lines.append(f'  - {m.group(1)} | {m.group(2)[:80]}')

# Try with looser regex (drop the lookahead)
pat2 = re.compile(r'#\s*路径([一二三四五六七八九十]+)[：:](.+?)(?=\n---|\n#|\Z)', re.DOTALL)
matches2 = list(pat2.finditer(line24))
lines.append(f'loose regex matches: {len(matches2)}')

# Even looser - just find all "# 路径N"
pat3 = re.compile(r'#\s*路径([一二三四五六七八九十]+)')
matches3 = list(pat3.finditer(line24))
lines.append(f'just header regex matches: {len(matches3)}')
for m in matches3:
    lines.append(f'  pos {m.start()}: {m.group(0)}')

with open('debug_out.txt', 'w', encoding='utf-8') as f:
    f.write('\n'.join(lines))

```
