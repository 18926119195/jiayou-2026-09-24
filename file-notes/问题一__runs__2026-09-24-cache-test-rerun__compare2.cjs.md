# compare2.cjs

> **路径**: `问题一\runs\2026-09-24-cache-test-rerun\compare2.cjs`  
> **分类**: 代码  
> **大小**: 1.0 KB  
> **最后修改**: 2026-09-24T11:45:58.088Z  

## 文件开头预览

```cjs
// compare2.cjs - compare call-0001 of Z1-Q1 vs Z1-Q2
const fs = require('fs');

const a = String.raw`C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-24-cache-test-rerun\snapshots\Z1-Q1\call-0001-prompt.txt`;
const b = String.raw`C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-24-cache-test-rerun\snapshots\Z1-Q2\call-0001-prompt.txt`;

const aText = fs.readFileSync(a, 'utf-8');
const bText = fs.readFileSync(b, 'utf-8');

console.log('Z1-Q1 prompt length:', aText.length);
console.log('Z1-Q2 prompt length:', bText.length);

let i = 0;
while (i < aText.length && i < bText.length && aText[i] === bText[i]) i++;
console.log('Common prefix length:', i, 'chars');

// Show the first different char
console.log('Z1-Q1 char at diff:', JSON.stringify(aText.substring(i-5, i+10)));
console.log('Z1-Q2 char at diff:', JSON.stringify(bText.substring(i-5, i+10)));
console.log('\nZ1-Q1 starts:', aText.substring(0, 100));
console.log('Z1-Q2 starts:', bText.substring(0, 100));

```
