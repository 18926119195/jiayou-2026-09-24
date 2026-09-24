# count3.ps1

> **路径**: `count3.ps1`  
> **分类**: 脚本  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T03:16:49.214Z  

## 文件开头预览

```ps1
$root = 'C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-23-cache-test-rerun\snapshots'
$files = Get-ChildItem -LiteralPath $root -Recurse -Filter 'call-*-response.json'
Write-Host ('Total files: ' + $files.Count)
$noneFiles = @()
$validFiles = @()
$scoreFiles = @()
$otherFiles = @()
foreach ($f in $files) {
    $raw = [System.IO.File]::ReadAllText($f.FullName, [System.Text.Encoding]::UTF8)
    if ($raw -match '"text":\s*"NONE"') { $noneFiles += $f }
    elseif ($raw -match '"text":\s*"【') { $validFiles += $f }
    elseif ($raw -match '"text":\s*"\s*') { $scoreFiles += $f }
    else { $otherFiles += $f }
}
Write-Host ('NONE: ' + $noneFiles.Count)
Write-Host ('Valid (starts with 【): ' + $validFiles.Count)
Write-Host ('Empty: ' + $scoreFiles.Count)
Write-Host ('Other: ' + $otherFiles.Count)
Write-Host ''
Write-Host '=== NONE files ==='
$noneFiles | ForEach-Object { Write-Host ($_.Directory.Name + ' ' + $_.Name) }
Write-Host ''
Write-Host '=== Other files ==='
$otherFiles | ForEach-Object { Write-Host ($_.Directory.Name + ' ' + $_.Name) }

```
