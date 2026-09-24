# compare-prev-vs-current.cjs

> **路径**: `问题一\runs\2026-09-24-cache-test-rerun\compare-prev-vs-current.cjs`  
> **分类**: 代码  
> **大小**: 1.8 KB  
> **最后修改**: 2026-09-24T11:46:09.044Z  

## 文件开头预览

```cjs
// compare-prev-vs-current.cjs
const fs = require('fs');

// Previous run: Z1-Q2 (after Z1-Q1 was run in the morning)
const prevZ1Q2 = String.raw`C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-23-cache-test-rerun-remainder\snapshots\Z1-Q2\call-0001-prompt.txt`;
const prevZ1Q2Resp = String.raw`C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-23-cache-test-rerun-remainder\snapshots\Z1-Q2\call-0001-response.json`;

// Current run: Z1-Q2 (no prior Z1-Q1 in cache)
const curZ1Q2 = String.raw`C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-24-cache-test-rerun\snapshots\Z1-Q2\call-0001-prompt.txt`;
const curZ1Q2Resp = String.raw`C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-24-cache-test-rerun\snapshots\Z1-Q2\call-0001-response.json`;

const prevText = fs.readFileSync(prevZ1Q2, 'utf-8');
const curText = fs.readFileSync(curZ1Q2, 'utf-8');

console.log('Previous Z1-Q2 (Sept 23) prompt length:', prevText.length);
console.log('Current Z1-Q2 (Sept 24) prompt length:', curText.length);

let i = 0;
while (i < prevText.length && i < curText.length && prevText[i] === curText[i]) i++;
console.log('Common prefix length:', i, 'chars');
console.log('Common prefix:', JSON.stringify(prevText.substring(0, i)));
console.log('First diff at:', JSON.stringify(prevText.substring(i, i+50)), 'vs', JSON.stringify(curText.substring(i, i+50)));

const prevResp = JSON.parse(fs.readFileSync(prevZ1Q2Resp, 'utf-8'));
const curResp = JSON.parse(fs.readFileSync(curZ1Q2Resp, 'utf-8'));
console.log('\nPrevious Z1-Q2 cache:', prevResp.response.usage.prompt_cache_hit_tokens, '/', prevResp.response.usage.prompt_tokens);
console.log('Current Z1-Q2 cache:', curResp.response.usage.prompt_cache_hit_tokens || 0, '/', curResp.response.usage.prompt_tokens);

```
