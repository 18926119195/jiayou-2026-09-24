# debug_paths.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\debug_paths.ps1`  
> **分类**: 脚本  
> **大小**: 0.7 KB  
> **最后修改**: 2026-09-24T11:57:50.753Z  

## 文件开头预览

```ps1
$raw = [System.IO.File]::ReadAllText("reasoning-output-Z2-Q2.json", [System.Text.Encoding]::UTF8)
$data = $raw | ConvertFrom-Json
$l24 = [string]$data.llmOutput
Write-Host "L24 length: $($l24.Length)"
Write-Host "First 300 chars of L24:"
Write-Host $l24.Substring(0, [Math]::Min(300, $l24.Length))
Write-Host ""
Write-Host "Looking for # character:"
$firstHash = $l24.IndexOf("#")
Write-Host "First # at: $firstHash"
if ($firstHash -ge 0) {
    $window = $l24.Substring($firstHash, [Math]::Min(50, $l24.Length - $firstHash))
    Write-Host "Window: $window"
    Write-Host "Matches 路徑: $($window -match '路徑')"
    Write-Host "Matches 路径: $($window -match '路径')"
    Write-Host "Matches path: $($window -match '#\s*路径')"
}

```
