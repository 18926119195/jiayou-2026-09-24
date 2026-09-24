# count4.ps1

> **路径**: `count4.ps1`  
> **分类**: 脚本  
> **大小**: 0.9 KB  
> **最后修改**: 2026-09-24T03:17:23.873Z  

## 文件开头预览

```ps1
$root = 'C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-23-cache-test-rerun\snapshots'
$files = Get-ChildItem -LiteralPath $root -Recurse -Filter 'call-*-response.json'
Write-Host ('Total files: ' + $files.Count)
$noneFiles = @()
$validFiles = @()
$otherFiles = @()
foreach ($f in $files) {
    $raw = [System.IO.File]::ReadAllText($f.FullName, [System.Text.Encoding]::UTF8)
    if ($raw -match 'text.:\s*.NONE.') { $noneFiles += $f }
    elseif ($raw -match 'text.:\s*.【') { $validFiles += $f }
    else { $otherFiles += $f }
}
Write-Host ('NONE: ' + $noneFiles.Count)
Write-Host ('Valid: ' + $validFiles.Count)
Write-Host ('Other: ' + $otherFiles.Count)
Write-Host ''
Write-Host '=== NONE files ==='
$noneFiles | ForEach-Object { Write-Host ($_.Directory.Name + ' ' + $_.Name) }
Write-Host ''
Write-Host '=== Other files ==='
$otherFiles | ForEach-Object { Write-Host ($_.Directory.Name + ' ' + $_.Name) }

```
