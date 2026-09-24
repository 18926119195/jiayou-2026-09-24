# debug_v2.py

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\debug_v2.py`  
> **分类**: 代码  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T10:15:49.941Z  

## 文件开头预览

```py
import json
import re

with open(r'C:\Users\Administrator\Desktop\chenggong-jiachi-master\cot对比实验\提高缓存命中率的实验\llm-configs\reasoning-output-Z1-Q3.json', 'r', encoding='utf-8') as f:
    data = json.load(f)

line23 = data[22]
line24 = data[23]

lines = []
lines.append(f'L23 length: {len(line23)}')
lines.append(f'L24 length: {len(line24)}')

# Test simple regex
hits = re.findall(r'#\s*路径[一二三四五六七八九十]', line24)
lines.append(f'simple regex hits: {len(hits)} -> {hits}')

# Test the full regex
pat = re.compile(r'#\s*路径([一二三四五六七八九十]+)[：:](.+?)(?=\n---+|\n#|\Z)', re.DOTALL)
matches = list(pat.finditer(line24))
lines.append(f'full regex matches: {len(matches)}')

# Just find all "# 路径N"
pat3 = re.compile(r'#\s*路径([一二三四五六七八九十]+)')
matches3 = list(pat3.finditer(line24))
lines.append(f'just header regex matches: {len(matches3)}')
for m in matches3:
    lines.append(f'  pos {m.start()}: {m.group(0)}')

# Show actual content around position 18 (where # 路径一 should be)
lines.append(f'')
lines.append(f'L24 chars 0-100: {repr(line24[:100])}')
lines.append(f'L24 chars 18-50: {repr(line24[18:50])}')

with open(r'C:\Users\Administrator\Desktop\chenggong-jiachi-master\cot对比实验\提高缓存命中率的实验\llm-configs\debug_out.txt', 'w', encoding='utf-8') as f:
    f.write('\n'.join(lines))

```
