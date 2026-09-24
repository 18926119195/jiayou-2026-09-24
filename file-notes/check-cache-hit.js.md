# check-cache-hit.js

> **路径**: `check-cache-hit.js`  
> **分类**: 代码  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T10:22:48.619Z  

## 文件开头预览

```js
import fs from 'fs';
import path from 'path';

const dir = path.join(process.cwd(), 'snapshots');
const files = fs.readdirSync(dir).filter(f => f.endsWith('-response.json'));

let totalHit = 0;
let totalMiss = 0;
let callsWithHit = 0;
const rows = [];

for (const f of files) {
  const data = JSON.parse(fs.readFileSync(path.join(dir, f), 'utf-8'));
  const usage = data.response?.usage;
  if (!usage) continue;
  const hit = usage.prompt_cache_hit_tokens || 0;
  const miss = usage.prompt_cache_miss_tokens || 0;
  totalHit += hit;
  totalMiss += miss;
  if (hit > 0) callsWithHit++;
  rows.push({ callId: data.callId, hit, miss });
}

const total = totalHit + totalMiss;
const rate = total > 0 ? (totalHit / total * 100).toFixed(2) : '0.00';

console.log(`总调用数: ${rows.length}`);
console.log(`有缓存命中的调用数: ${callsWithHit}`);
console.log(`总 cache_hit_tokens: ${totalHit}`);
console.log(`总 cache_miss_tokens: ${totalMiss}`);
console.log(`整体缓存命中率: ${rate}%`);

if (callsWithHit > 0) {
  console.log('\n有命中的调用示例:');
  rows.filter(r => r.hit > 0).slice(0, 10).forEach(r => {
    console.log(`  ${r.callId}: hit=${r.hit} miss=${r.miss}`);
  });
}

```
