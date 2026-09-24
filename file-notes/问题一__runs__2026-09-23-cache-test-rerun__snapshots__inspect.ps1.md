# inspect.ps1

> **路径**: `问题一\runs\2026-09-23-cache-test-rerun\snapshots\inspect.ps1`  
> **分类**: 脚本  
> **大小**: 0.6 KB  
> **最后修改**: 2026-09-24T03:02:05.631Z  

## 文件开头预览

```ps1
$ErrorActionPreference = 'SilentlyContinue'
Set-Location 'Z1-Q1'
$j = Get-Content 'call-0001-response.json' -Raw | ConvertFrom-Json
Write-Host "callId: $($j.callId)"
Write-Host "response.text: [$($j.response.text)]"
Write-Host "Length: $($j.response.text.Length)"
$t = $j.response.text
Write-Host "eq NONE: $($t -eq 'NONE')"
Write-Host "starts with [【]: $($t.StartsWith([char]0x3010))"
Write-Host "First char hex: $('{0:X4}' -f [int]$t[0])"
Write-Host "Char codes:"
[byte[]]$bytes = [System.Text.Encoding]::UTF8.GetBytes($t.Substring(0,4))
$bytes | ForEach-Object { Write-Host ("  " + ('{0:X2}' -f $_)) }

```
