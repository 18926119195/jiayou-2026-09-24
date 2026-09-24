# inspect-z1q1.cjs

> **路径**: `问题一\runs\2026-09-24-cache-test-rerun\inspect-z1q1.cjs`  
> **分类**: 代码  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T11:46:27.217Z  

## 文件开头预览

```cjs
// inspect-z1q1.cjs - inspect first call cache info from full run
const fs = require('fs');

const resp = JSON.parse(fs.readFileSync(String.raw`C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-24-cache-test-rerun\snapshots\Z1-Q1\call-0001-response.json`, 'utf-8'));
console.log('Full run Z1-Q1 call-0001:');
console.log('  prompt_tokens:', resp.response.usage.prompt_tokens);
console.log('  prompt_cache_hit_tokens:', resp.response.usage.prompt_cache_hit_tokens);
console.log('  prompt_cache_miss_tokens:', resp.response.usage.prompt_cache_miss_tokens);

console.log('\nFirst 5 calls of Z1-Q1 (cache info):');
for (let i = 1; i <= 5; i++) {
  const fn = String.raw`C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-24-cache-test-rerun\snapshots\Z1-Q1\call-${String(i).padStart(4, '0')}-response.json`;
  const data = JSON.parse(fs.readFileSync(fn, 'utf-8'));
  const u = data.response.usage;
  console.log(`  call-${String(i).padStart(4, '0')}: prompt=${u.prompt_tokens} cached=${u.prompt_cache_hit_tokens} miss=${u.prompt_cache_miss_tokens} (${(u.prompt_cache_hit_tokens / u.prompt_tokens * 100).toFixed(1)}%)`);
}

```
