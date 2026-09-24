# verify-citation-mapping.js

> **路径**: `cot对比实验\提高缓存命中率的实验\verify-citation-mapping.js`  
> **分类**: 代码  
> **大小**: 4.1 KB  
> **最后修改**: 2026-09-24T08:35:02.592Z  

## 文件开头预览

```js
import fs from 'fs';
import path from 'path';
import { fileURLToPath } from 'url';

const __filename = fileURLToPath(import.meta.url);
const __dirname = path.dirname(__filename);

const configDir = 'c:\\Users\\Administrator\\Desktop\\chenggong-jiachi-master\\cot对比实验\\提高缓存命中率的实验\\llm-configs';

// 提取所有【【数字】】格式的引用
function extractCitations(text) {
    const regex = /【【(\d+)】】/g;
    const citations = new Set();
    let match;
    while ((match = regex.exec(text)) !== null) {
        citations.add(match[1]);
    }
    return Array.from(citations).sort((a, b) => parseInt(a) - parseInt(b));
}

// 检查单个文件
function verifyFile(filepath) {
    const content = fs.readFileSync(filepath, 'utf8');
    const data = JSON.parse(content);
    
    const thinkingCitations = extractCitations(data.thinkingChain || '');
    const outputCitations = extractCitations(data.llmOutput || '');
    
    // 检查 output 中的引用是否都在 thinking 中出现过
    const missingInThinking = outputCitations.filter(c => !thinkingCitations.includes(c));
    const onlyInThinking = thinkingCitations.filter(c => !outputCitations.includes(c));
    
    return {
        filename: path.basename(filepath),
        thinkingCount: thinkingCitations.length,
        outputCount: outputCitations.length,
        thinkingCitations,
        outputCitations,
        missingInThinking, // output中有但thinking中没有的
        onlyInThinking,    // thinking中有但output中没有的
        coverage: outputCitations.length > 0 
            ? ((outputCitations.length - missingInThinking.length) / outputCitations.length * 100).toFixed(1)
            : '100.0'
    };
}

// 主函数
function main() {
    const files = fs.readdirSync(configDir)
        .filter(f => f.startsWith('reasoning-output-Z') && f.endsWith('.json'))
```
