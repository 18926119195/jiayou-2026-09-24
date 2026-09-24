# inspect3.ps1

> **路径**: `问题一\runs\2026-09-23-cache-test-rerun\snapshots\inspect3.ps1`  
> **分类**: 脚本  
> **大小**: 0.3 KB  
> **最后修改**: 2026-09-24T03:04:25.018Z  

## 文件开头预览

```ps1
$ErrorActionPreference = 'Continue'
$utf8 = New-Object System.Text.UTF8Encoding $false
$baseDir = 'C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-23-cache-test-rerun\snapshots\Z1-Q1'
Set-Location $baseDir
Write-Host "PWD: $PWD"
Write-Host "Files in CWD:"
Get-ChildItem -Name | Select-Object -First 5

```
