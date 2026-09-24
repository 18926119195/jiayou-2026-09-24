# chunk_overlap_check.mjs

> **路径**: `chunk_overlap_check.mjs`  
> **分类**: 代码  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T05:36:28.493Z  

## 文件开头预览

```mjs
import { readFileSync, writeFileSync } from 'fs';

const path = 'C:/Users/Administrator/Desktop/chenggong-jiachi-master/\u95EE\u9898\u4E00/runs/2026-09-23-cache-test-rerun-remainder/final/material-traceback-map.json';
const data = JSON.parse(readFileSync(path, 'utf-8'));

const qids = Object.keys(data);
const chunkSets = {};
for (const qid of qids) {
  const mats = data[qid].materials;
  chunkSets[qid] = new Set(Object.values(mats).map(m => m.chunkKey));
}

const lines = [];
lines.push('\u95EE\u9898\u6570: ' + qids.length);
for (const qid of qids) {
  lines.push(qid + ' chunk\u6570: ' + chunkSets[qid].size);
}

lines.push('---\u4E24\u4E24\u91CD\u5408\u7387(overlap>0)---');
let anyOverlap = false;
for (let i = 0; i < qids.length; i++) {
  for (let j = i + 1; j < qids.length; j++) {
    const a = chunkSets[qids[i]];
    const b = chunkSets[qids[j]];
    let overlap = 0;
    for (const k of a) if (b.has(k)) overlap++;
    if (overlap > 0) {
      anyOverlap = true;
      const rate = (overlap / Math.min(a.size, b.size) * 100).toFixed(1);
      lines.push(qids[i] + ' vs ' + qids[j] + ': overlap=' + overlap + ' rate=' + rate + '%');
    }
  }
}
if (!anyOverlap) lines.push('(\u6CA1\u6709\u4EFB\u4F55\u4E24\u4E2A\u95EE\u9898\u5171\u4EAB\u540C\u4E00\u4E2AchunkKey)');

const out = lines.join('\n');
writeFileSync('C:/Users/Administrator/Desktop/chenggong-jiachi-master/chunk_overlap_result.txt', out, 'utf-8');
process.stdout.write(out + '\n');

```
