# count5.ps1

> **路径**: `count5.ps1`  
> **分类**: 脚本  
> **大小**: 0.9 KB  
> **最后修改**: 2026-09-24T03:17:42.115Z  

## 文件开头预览

```ps1
$root = 'C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-23-cache-test-rerun\snapshots'
$files = Get-ChildItem -LiteralPath $root -Recurse -Filter 'call-*-response.json'
$total = $files.Count
$noneCount = 0
$validCount = 0
$otherCount = 0
$noneList = @()
$otherList = @()
foreach ($f in $files) {
    $raw = [System.IO.File]::ReadAllText($f.FullName, [System.Text.Encoding]::UTF8)
    if ($raw -match 'text.:\s*.NONE.') {
        $noneCount++
        $noneList += $f.Directory.Name + '/' + $f.Name
    } elseif ($raw -match 'text.:\s*.【') {
        $validCount++
    } else {
        $otherCount++
        $otherList += $f.Directory.Name + '/' + $f.Name
    }
}
Write-Host ('Total=' + $total)
Write-Host ('NONE=' + $noneCount)
Write-Host ('Valid=' + $validCount)
Write-Host ('Other=' + $otherCount)
Write-Host '==NONE=='
$noneList | ForEach-Object { Write-Host $_ }
Write-Host '==Other=='
$otherList | ForEach-Object { Write-Host $_ }

```
