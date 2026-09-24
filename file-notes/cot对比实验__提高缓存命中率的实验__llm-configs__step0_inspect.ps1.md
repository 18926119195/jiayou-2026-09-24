# step0_inspect.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\step0_inspect.ps1`  
> **分类**: 脚本  
> **大小**: 0.8 KB  
> **最后修改**: 2026-09-24T11:50:27.880Z  

## 文件开头预览

```ps1
$ErrorActionPreference = 'Stop'
$files = @('reasoning-output-Z2-Q2.json','reasoning-output-Z2-Q3.json','reasoning-output-Z2-Q4.json','reasoning-output-Z3-Q3.json','reasoning-output-Z4-Q3.json')
Write-Host "================================================================================"
Write-Host "FILE INSPECTION"
Write-Host "================================================================================"
foreach ($f in $files) {
    if (Test-Path $f) {
        $r = [System.IO.File]::ReadAllText($f, [System.Text.Encoding]::UTF8)
        $d = $r | ConvertFrom-Json
        $l23 = [string]$d.thinkingChain
        $l24 = [string]$d.llmOutput
        Write-Host ""
        Write-Host $f
        Write-Host ("  L23 chars: " + $l23.Length)
        Write-Host ("  L24 chars: " + $l24.Length)
    } else {
        Write-Host ("NOT FOUND: " + $f)
    }
}

```
