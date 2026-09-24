# inspect4.ps1

> **路径**: `问题一\runs\2026-09-23-cache-test-rerun\snapshots\inspect4.ps1`  
> **分类**: 脚本  
> **大小**: 0.6 KB  
> **最后修改**: 2026-09-24T03:05:05.819Z  

## 文件开头预览

```ps1
chcp 65001 | Out-Null
$baseDir = 'C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-23-cache-test-rerun\snapshots\Z1-Q1'
Set-Location -LiteralPath $baseDir
Write-Host "PWD: $PWD"
$f = 'call-0001-response.json'
if (Test-Path $f) {
    $j = Get-Content -LiteralPath $f -Raw | ConvertFrom-Json
    Write-Host "callId: $($j.callId)"
    Write-Host ("text len: " + $j.response.text.Length)
    Write-Host ("first 80: " + $j.response.text.Substring(0, [Math]::Min(80, $j.response.text.Length)))
} else {
    Write-Host "File not found"
    Get-ChildItem -Name | Select-Object -First 5
}

```
