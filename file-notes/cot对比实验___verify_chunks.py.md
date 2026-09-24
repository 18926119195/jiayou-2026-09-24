# _verify_chunks.py

> **路径**: `cot对比实验\_verify_chunks.py`  
> **分类**: 代码  
> **大小**: 1.7 KB  
> **最后修改**: 2026-09-24T03:55:57.224Z  

## 文件开头预览

```py
# 验证 chunks 部分在 15 个文件中是否完全相同
import os

MARKER = '【【全量材料】】'
DIR = r'C:\Users\Administrator\Desktop\chenggong-jiachi-master\cot对比实验'
FILES = [
    'multipath-prompt-cot-Z1-Q1.txt',
    'multipath-prompt-cot-Z1-Q2.txt',
    'multipath-prompt-cot-Z1-Q3.txt',
    'multipath-prompt-cot-Z1-Q4.txt',
    'multipath-prompt-cot-Z2-Q1.txt',
    'multipath-prompt-cot-Z2-Q2.txt',
    'multipath-prompt-cot-Z2-Q3.txt',
    'multipath-prompt-cot-Z2-Q4.txt',
    'multipath-prompt-cot-Z3-Q1.txt',
    'multipath-prompt-cot-Z3-Q2.txt',
    'multipath-prompt-cot-Z3-Q3.txt',
    'multipath-prompt-cot-Z4-Q1.txt',
    'multipath-prompt-cot-Z4-Q2.txt',
    'multipath-prompt-cot-Z4-Q3.txt',
    'multipath-prompt-cot-Z4-Q4.txt',
]

def get_chunks(path):
    with open(path, 'r', encoding='utf-8') as f:
        s = f.read()
    idx = s.find(MARKER)
    return idx, s[idx:]

# 检查 chunks 部分是否完全相同
chunks_parts = {}
for fn in FILES:
    idx, c = get_chunks(os.path.join(DIR, fn))
    chunks_parts[fn] = (idx, c)

print('== 各文件 header / chunks 长度 ==')
for fn in FILES:
    idx, c = chunks_parts[fn]
    print(f'  {fn}: 总长={idx + len(c):,}  header={idx:,}  chunks={len(c):,}')


print('\n== chunks 部分是否完全一致 ==')
ref_fn = FILES[0]
ref_chunks = chunks_parts[ref_fn][1]
print(f'基准文件: {ref_fn}')
print(f'基准 chunks 字节数: {len(ref_chunks):,}')
all_same = True
for fn in FILES[1:]:
    c = chunks_parts[fn][1]
    same = (c == ref_chunks)
```
