# cache-rate.cjs

> **路径**: `问题一\runs\2026-09-24-cache-test-rerun\cache-rate.cjs`  
> **分类**: 代码  
> **大小**: 1.6 KB  
> **最后修改**: 2026-09-24T11:45:46.670Z  

## 文件开头预览

```cjs
// cache-rate.cjs - compute cache hit rate per question
const fs = require('fs');
const path = require('path');

const SNAP_DIR = String.raw`C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-24-cache-test-rerun\snapshots`;

const qids = fs.readdirSync(SNAP_DIR).filter(d => d.startsWith('Z') && fs.statSync(path.join(SNAP_DIR, d)).isDirectory()).sort();
console.log('QID           calls  prompt_tok  cached_tok  hit_rate');
console.log('-'.repeat(60));
let grandPrompt = 0, grandCached = 0;
for (const qid of qids) {
  const qdir = path.join(SNAP_DIR, qid);
  const responseFiles = fs.readdirSync(qdir).filter(f => /call-\d{4}-response\.json$/.test(f)).sort();
  let pt = 0, ct = 0;
  for (const f of responseFiles) {
    const data = JSON.parse(fs.readFileSync(path.join(qdir, f), 'utf-8'));
    const u = data.response?.usage;
    if (u) {
      pt += u.prompt_tokens || 0;
      ct += u.prompt_cache_hit_tokens || 0;
    }
  }
  grandPrompt += pt;
  grandCached += ct;
  const rate = pt > 0 ? (ct / pt * 100).toFixed(2) : 'N/A';
  console.log(`${qid.padEnd(13)}  ${String(responseFiles.length).padStart(4)}  ${String(pt).padStart(9)}  ${String(ct).padStart(9)}  ${rate}%`);
}
console.log('-'.repeat(60));
const overall = grandPrompt > 0 ? (grandCached / grandPrompt * 100).toFixed(2) : 'N/A';
console.log(`${'TOTAL'.padEnd(13)}  ${String(qids.reduce((s, q) => s + fs.readdirSync(path.join(SNAP_DIR, q)).filter(f => /call-\d{4}-response\.json$/.test(f)).length, 0)).padStart(4)}  ${String(grandPrompt).padStart(9)}  ${String(grandCached).padStart(9)}  ${overall}%`);

```
