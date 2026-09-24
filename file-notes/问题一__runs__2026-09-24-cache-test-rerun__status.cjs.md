# status.cjs

> **路径**: `问题一\runs\2026-09-24-cache-test-rerun\status.cjs`  
> **分类**: 代码  
> **大小**: 0.7 KB  
> **最后修改**: 2026-09-24T11:45:37.009Z  

## 文件开头预览

```cjs
// status.cjs - check pipeline progress
const fs = require('fs');

const log = String.raw`C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-24-cache-test-rerun\logs\runner-stdout.log`;
const txt = fs.readFileSync(log, 'utf-8');
const lines = txt.split(/\r?\n/);

console.log('total lines:', lines.length);
const coarseDone = lines.filter(l => l.includes('粗筛完成'));
console.log('粗筛完成 lines:', coarseDone.length);
const reasoningDone = lines.filter(l => l.includes('推理完成'));
console.log('推理完成 lines:', reasoningDone.length);

const last5 = lines.slice(-15);
console.log('\nLast 15 lines:');
for (const l of last5) console.log('  ' + l);

```
