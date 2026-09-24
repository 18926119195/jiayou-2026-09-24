# test_path.ps1

> **路径**: `test_path.ps1`  
> **分类**: 脚本  
> **大小**: 0.5 KB  
> **最后修改**: 2026-09-24T03:06:00.414Z  

## 文件开头预览

```ps1
$f = 'C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-23-cache-test-rerun\snapshots\Z1-Q1\call-0001-response.json'
if (Test-Path -LiteralPath $f) {
    $j = Get-Content -LiteralPath $f -Raw | ConvertFrom-Json
    Write-Host ("callId: " + $j.callId)
    Write-Host ("text len: " + $j.response.text.Length)
    Write-Host ("first 100: " + $j.response.text.Substring(0, [Math]::Min(100, $j.response.text.Length)))
} else {
    Write-Host "not found"
}

```
