# chunk_overlap_check.py

> **路径**: `chunk_overlap_check.py`  
> **分类**: 代码  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T05:26:40.412Z  

## 文件开头预览

```py
import json

path = r'C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-23-cache-test-rerun-remainder\final\material-traceback-map.json'
with open(path, encoding='utf-8') as f:
    data = json.load(f)

qids = list(data.keys())
chunk_sets = {}
for qid in qids:
    mats = data[qid]['materials']
    chunk_sets[qid] = set(m['chunkKey'] for m in mats.values())

lines = []
lines.append('问题数: ' + str(len(qids)))
for qid in qids:
    lines.append(qid + ' chunk数: ' + str(len(chunk_sets[qid])))

lines.append('---两两重合率(overlap>0)---')
any_overlap = False
for i in range(len(qids)):
    for j in range(i + 1, len(qids)):
        a, b = chunk_sets[qids[i]], chunk_sets[qids[j]]
        overlap = len(a & b)
        if overlap > 0:
            any_overlap = True
            rate = overlap / min(len(a), len(b)) * 100
            lines.append(qids[i] + ' vs ' + qids[j] + ': overlap=' + str(overlap) + ' rate=%.1f%%' % rate)
if not any_overlap:
    lines.append('(没有任何两个问题共享同一个chunkKey)')

out = '\n'.join(lines)
out_path = r'C:\Users\Administrator\Desktop\chenggong-jiachi-master\chunk_overlap_result.txt'
with open(out_path, 'w', encoding='utf-8') as f:
    f.write(out)
print(out)

```
