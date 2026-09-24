# count6.ps1

> **路径**: `count6.ps1`  
> **分类**: 脚本  
> **大小**: 0.9 KB  
> **最后修改**: 2026-09-24T03:18:01.642Z  

## 文件开头预览

```ps1
$root = 'C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-23-cache-test-rerun\snapshots'
$out = 'C:\Users\Administrator\Desktop\chenggong-jiachi-master\count_out.txt'
$files = Get-ChildItem -LiteralPath $root -Recurse -Filter 'call-*-response.json'
$total = $files.Count
$noneCount = 0
$validCount = 0
$otherCount = 0
$lines = @()
$lines += ("Total=" + $total)
foreach ($f in $files) {
    $raw = [System.IO.File]::ReadAllText($f.FullName, [System.Text.Encoding]::UTF8)
    $name = $f.Directory.Name + "/" + $f.Name
    if ($raw -match 'text.:\s*.NONE.') {
        $noneCount++
        $lines += ("NONE " + $name)
    } elseif ($raw -match 'text.:\s*.【') {
        $validCount++
    } else {
        $otherCount++
        $lines += ("OTHER " + $name)
    }
}
$lines += ("NONE_COUNT=" + $noneCount)
$lines += ("VALID_COUNT=" + $validCount)
$lines += ("OTHER_COUNT=" + $otherCount)
$lines | Out-File -LiteralPath $out -Encoding UTF8

```
