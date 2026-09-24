# demo_match.py

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\demo_match.py`  
> **分类**: 代码  
> **大小**: 2.5 KB  
> **最后修改**: 2026-09-24T08:53:56.334Z  

## 文件开头预览

```py
import re
from collections import Counter

import os
import sys
import traceback
os.chdir(r'c:\Users\Administrator\Desktop\chenggong-jiachi-master\cot对比实验\提高缓存命中率的实验\llm-configs')
sys.stdout.reconfigure(encoding='utf-8')
filepath = 'reasoning-output-Z1-Q3.json'

try:
    with open(filepath, 'r', encoding='utf-8') as f:
        lines = f.readlines()
except Exception as e:
    print(f'ERROR opening file: {e}', flush=True)
    traceback.print_exc()
    sys.exit(1)

line23 = lines[22]  # 0-indexed: line 23
line24 = lines[23]  # 0-indexed: line 24

print(f'L23 length: {len(line23)} chars')
print(f'L24 length: {len(line24)} chars')
print('---')

# 1. Extract all 【N】 from L23 (thinking chain)
matches23 = list(re.finditer(r'【(\d+)】', line23))
counter23 = Counter(m.group(1) for m in matches23)
print(f'L23 total 【N】 matches: {len(matches23)}')
print(f'L23 unique numbers: {len(counter23)} → {sorted(counter23.keys(), key=int)}')

# 2. Extract all 【【N】】 from L24 (final output)
matches24 = list(re.finditer(r'【【(\d+)】】', line24))
counter24 = Counter(m.group(1) for m in matches24)
print(f'\nL24 total 【【N】】 matches: {len(matches24)}')
print(f'L24 unique numbers: {len(counter24)} → {sorted(counter24.keys(), key=int)}')

# 3. Show: L24 numbers that are NOT in L23 (hallucinated?)
missing_in_L23 = set(counter24.keys()) - set(counter23.keys())
extra_in_L23 = set(counter23.keys()) - set(counter24.keys())
print(f'\nL24 references NOT found in L23 (potential hallucinations): {missing_in_L23}')
print(f'L23 references NOT used in L24 (dropped during generation): {sorted(extra_in_L23, key=int)}')

# 4. Demonstrate: For each L24 number, find ALL matching positions in L23 with context
print('\n' + '='*80)
print('DEMO: For 【【224】】 (appears 13x in L23), show ALL positions with context:')
print('='*80)
for m in re.finditer(r'【224】', line23):
    pos = m.start()
    start = max(0, pos - 80)
```
