# runner.cjs

> **路径**: `问题一\runs\2026-09-24-cache-test-rerun\runner.cjs`  
> **分类**: 代码  
> **大小**: 8.8 KB  
> **最后修改**: 2026-09-24T11:38:14.021Z  

## 文件开头预览

```cjs
// runner.cjs - main entry point that handles Chinese path encoding correctly
// This script reads its config and invokes the actual scripts via spawn

const { spawn } = require('child_process');
const fs = require('fs');
const path = require('path');

// Use Buffer to ensure correct UTF-8 byte sequences for Chinese characters
function toPath(parts) {
  return parts.map(p => Buffer.from(p, 'utf-8').toString('utf-8')).join(path.sep);
}

const ROOT_RAW = 'C:\\Users\\Administrator\\Desktop\\chenggong-jiachi-master';
const SRC_DIR_RAW = ROOT_RAW + '\\完整的运作';
const RUN_DIR_RAW = ROOT_RAW + '\\问题一\\runs\\2026-09-24-cache-test-rerun';
const NODE_EXE = 'C:\\PROGRA~1\\nodejs\\node.exe';

const SRC_DIR = toPath([SRC_DIR_RAW]);
const RUN_DIR = toPath([RUN_DIR_RAW]);
const LOG_DIR = path.join(RUN_DIR, 'logs');
const SNAPSHOT_DIR = path.join(RUN_DIR, 'snapshots');
const FINAL_DIR = path.join(RUN_DIR, 'final');

function loadEnv() {
  const envPath = Buffer.from(ROOT_RAW + '\\.env', 'utf-8').toString('utf-8');
  const content = fs.readFileSync(envPath, 'utf-8');
  for (const line of content.split('\n')) {
    const m = line.match(/^\s*([A-Z_][A-Z0-9_]*)\s*=\s*(.*?)\s*$/);
    if (m && !m[1].startsWith('#')) {
      const [, name, value] = m;
      process.env[name] = value;
    }
  }
}

function appendLog(file, text) {
  fs.appendFileSync(file, text + '\n', 'utf-8');
}

function nowStr() {
  return new Date().toISOString().replace('T', ' ').slice(0, 19);
}

function runNode(script, args, logFile, env = {}) {
  return new Promise((resolve, reject) => {
    const child = spawn(NODE_EXE, [script, ...args], {
      cwd: SRC_DIR,
      env: { ...process.env, ...env },
      stdio: ['ignore', 'pipe', 'pipe'],
    });
```
