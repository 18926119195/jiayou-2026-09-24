# count_all2.ps1

> **路径**: `count_all2.ps1`  
> **分类**: 脚本  
> **大小**: 1.1 KB  
> **最后修改**: 2026-09-24T03:09:24.366Z  

## 文件开头预览

```ps1
$root = 'C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-23-cache-test-rerun\snapshots'
$bracket = [string][char]0x3010
$open = $bracket + $bracket
$dirs = Get-ChildItem -LiteralPath $root -Directory
foreach ($d in $dirs) {
    Write-Host ('--- ' + $d.Name + ' ---')
    $files = Get-ChildItem -LiteralPath $d.FullName -Filter 'call-*-response.json' | Sort-Object Name
    $total = 0; $none = 0; $score = 0; $valid = 0; $other = 0
    $unknowns = @()
    foreach ($f in $files) {
        $total++
        $j = Get-Content -LiteralPath $f.FullName -Raw | ConvertFrom-Json
        $t = $j.response.text
        $firstTwo = $t.Substring(0, [Math]::Min(4, $t.Length))
        if ($t -eq 'NONE') {
            $none++
        } elseif ($t.StartsWith($open)) {
            $valid++
        } else {
            $other++
            $unknowns += ($f.Name + ' :: first=' + $firstTwo)
        }
    }
    Write-Host ('Total=' + $total + ' Valid(open-bracket)=' + $valid + ' NONE=' + $none + ' Other=' + $other)
    foreach ($u in $unknowns) { Write-Host ('  ' + $u) }
}

```
