# generate-mds.cjs

> **路径**: `generate-mds.cjs`  
> **分类**: 代码  
> **大小**: 15.0 KB  
> **最后修改**: 2026-09-24T12:17:45.963Z  

## 文件开头预览

```cjs
// generate-mds.js
// Generate markdown navigation for everything modified today (2026-09-24)
const fs = require('fs');
const path = require('path');

const ROOT = process.argv[2] || 'C:\\Users\\Administrator\\Desktop\\chenggong-jiachi-master';
const TRANSCRIPT_ROOT = 'C:\\Users\\Administrator\\.cursor\\projects\\c-Users-Administrator-Desktop-chenggong-jiachi-master';
const OUT = ROOT;

const TODAY = new Date('2026-09-24T00:00:00');

function isToday(d) {
    const t = new Date(d);
    return t >= TODAY;
}

function safeRead(p) {
    try { return fs.readFileSync(p, 'utf8'); } catch (e) { return null; }
}

function safeStat(p) {
    try { return fs.statSync(p); } catch (e) { return null; }
}

function safeReaddir(p) {
    try { return fs.readdirSync(p, { withFileTypes: true }); } catch (e) { return []; }
}

// Walk and collect files
function walk(dir, exclude, results = []) {
    const entries = safeReaddir(dir);
    for (const e of entries) {
        if (exclude.includes(e.name)) continue;
        const full = path.join(dir, e.name);
        if (e.isDirectory()) {
            walk(full, exclude, results);
        } else if (e.isFile()) {
            const st = safeStat(full);
            if (st && isToday(st.mtime)) {
                results.push({ path: full, size: st.size, mtime: st.mtime });
            }
        }
    }
    return results;
}

const EXCLUDE_DIRS = ['node_modules', '.git', '.today-files.csv', '.today-top.csv', '.today-walk.csv', '.chats.csv', '.scan-today.ps1', '.scan-top.ps1', '.scan-walk.ps1', '.scan-chats.ps1'];

console.log('[scan] walking workspace...');
const todayFiles = walk(ROOT, EXCLUDE_DIRS);
```
