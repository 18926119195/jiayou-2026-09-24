# do_path_mapping.py

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\do_path_mapping.py`  
> **分类**: 代码  
> **大小**: 5.4 KB  
> **最后修改**: 2026-09-24T10:06:39.453Z  

## 文件开头预览

```py
# -*- coding: utf-8 -*-
import json, re, unicodedata

with open('reasoning-output-Z1-Q3.json', 'r', encoding='utf-8') as f:
    data = json.load(f)

line23 = data[22]  # L23 = index 22
line24 = data[23]  # L24 = index 23

LB = '\u3010'  # 【
RB = '\u3011'  # 】

ZH_TO_ARAB = {'\u4e00':'1', '\u4e8c':'2', '\u4e09':'3', '\u56db':'4',
              '\u4e94':'5', '\u516d':'6', '\u4e03':'7', '\u516b':'8',
              '\u4e5d':'9', '\u5341':'10'}

# ============================================================
# Parse L24 into path blocks
# ============================================================
# Match "# 路径N：...---" blocks
pattern24 = re.compile(
    r'#\s*路径([一二三四五六七八九十]+)[：:](.+?)(?=\n---+|\n#|\Z)',
    re.DOTALL
)
path_blocks_24 = []
for m in pattern24.finditer(line24):
    title = m.group(2).strip()
    full = m.group(0)
    # Find all [[N]] citations
    chunks = re.findall(r'\[\[(\d+)\]\]', full)
    path_blocks_24.append({
        'title': title,
        'full': full,
        'chunks': chunks
    })

# ============================================================
# Parse L23 into path blocks
# ============================================================
pattern23 = re.compile(r'#\s*路径([一二三四五六七八九十]+)[：:]')
ph23 = []
for m in pattern23.finditer(line23):
    ph23.append({'path_num': m.group(1), 'pos': m.start()})
ph23.sort(key=lambda x: x['pos'])

for i, p in enumerate(ph23):
    start = p['pos']
    end = ph23[i+1]['pos'] if i+1 < len(ph23) else len(line23)
    p['start'] = start
    p['end'] = end
```
