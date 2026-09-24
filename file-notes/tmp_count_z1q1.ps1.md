# tmp_count_z1q1.ps1

> **路径**: `tmp_count_z1q1.ps1`  
> **分类**: 脚本  
> **大小**: 0.9 KB  
> **最后修改**: 2026-09-24T02:56:49.608Z  

## 文件开头预览

```ps1
Set-Location -LiteralPath 'C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-23-cache-test-rerun\snapshots\Z1-Q1'
$files = Get-ChildItem -Filter 'call-*-response.json' | Sort-Object Name
$total = $files.Count
$noneCount = 0
$validCount = 0
$scoreCount = 0
$results = @()
foreach ($file in $files) {
    $j = Get-Content $file.FullName -Raw | ConvertFrom-Json
    $text = $j.response.text
    $preview = if ($text.Length -gt 80) { $text.Substring(0,80) + '...' } else { $text }
    $results += "$($j.callId) | $($j.elapsed)ms | $preview"
    if ($text -eq 'NONE') { $noneCount++ }
    elseif ($text -match '【【\d+】】\d+') { $scoreCount++ }
    else { $validCount++ }
}
Write-Host "Total: $total"
Write-Host "NONE: $noneCount"
Write-Host "Score format: $scoreCount"
Write-Host "Valid (noun selection): $validCount"
Write-Host ""
Write-Host "=== All responses ==="
$results | ForEach-Object { Write-Host $_ }

```
