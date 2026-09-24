# test.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\test.ps1`  
> **分类**: 脚本  
> **大小**: 0.2 KB  
> **最后修改**: 2026-09-24T10:21:13.893Z  

## 文件开头预览

```ps1
﻿\ = [System.IO.File]::ReadAllText(''reasoning-output-Z1-Q3.json'', [System.Text.Encoding]::UTF8)
\ = \ -split " \
\
\Length:\ + \.Count
\L24 first char index 23:\ + \[23].Substring(0, 50)
```
