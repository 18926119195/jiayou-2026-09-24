# debug3.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\debug3.ps1`  
> **分类**: 脚本  
> **大小**: 0.5 KB  
> **最后修改**: 2026-09-24T12:03:25.360Z  

## 文件开头预览

```ps1
$raw = [System.IO.File]::ReadAllText("reasoning-output-Z2-Q2.json", [System.Text.Encoding]::UTF8)
$data = $raw | ConvertFrom-Json
$l24 = $data.llmOutput
Write-Host "Type: $($l24.GetType().FullName)"
Write-Host "IsArray: $($l24 -is [array])"
if ($l24 -is [array]) {
    Write-Host "Count: $($l24.Count)"
    Write-Host "First: $($l24[0])"
} else {
    Write-Host "Length: $($l24.Length)"
    Write-Host "First 50: $($l24.Substring(0, [Math]::Min(50, $l24.Length)))"
    Write-Host "Char 0: |$($l24[0])| (code: $([int]$l24[0]))"
}

```
