# smoke-test.cjs

> **路径**: `问题一\runs\2026-09-24-cache-test-rerun\smoke-test.cjs`  
> **分类**: 代码  
> **大小**: 3.4 KB  
> **最后修改**: 2026-09-24T11:21:47.390Z  

## 文件开头预览

```cjs
// smoke-test.cjs - smoke test for one question to verify setup
const { spawn } = require('child_process');
const fs = require('fs');
const path = require('path');

const ROOT = String.raw`C:\Users\Administrator\Desktop\chenggong-jiachi-master`;
const SRC_DIR = path.join(ROOT, '完整的运作');
const RUN_DIR = path.join(ROOT, '问题一', 'runs', '2026-09-24-cache-test-rerun');
const NODE_EXE = String.raw`C:\Program Files\nodejs\node.exe`;

function loadEnv() {
  const envPath = path.join(ROOT, '.env');
  const content = fs.readFileSync(envPath, 'utf-8');
  for (const line of content.split('\n')) {
    const m = line.match(/^\s*([A-Z_][A-Z0-9_]*)\s*=\s*(.*?)\s*$/);
    if (m && !m[1].startsWith('#')) {
      const [, name, value] = m;
      process.env[name] = value;
    }
  }
}

function runNode(script, args, logFile, env = {}) {
  return new Promise((resolve, reject) => {
    const child = spawn(NODE_EXE, [script, ...args], {
      cwd: SRC_DIR,
      env: { ...process.env, ...env },
      stdio: ['ignore', 'pipe', 'pipe'],
    });
    const out = fs.openSync(logFile, 'a');
    child.stdout.on('data', (chunk) => {
      const text = chunk.toString('utf-8');
      process.stdout.write(text);
      fs.writeSync(out, text);
    });
    child.stderr.on('data', (chunk) => {
      const text = chunk.toString('utf-8');
      process.stderr.write(text);
      fs.writeSync(out, text);
    });
    child.on('error', reject);
    child.on('close', (code) => {
      fs.closeSync(out);
      resolve(code);
    });
  });
}

async function main() {
  loadEnv();
```
