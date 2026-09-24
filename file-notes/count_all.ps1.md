# count_all.ps1

> **路径**: `count_all.ps1`  
> **分类**: 脚本  
> **大小**: 1.2 KB  
> **最后修改**: 2026-09-24T03:08:30.469Z  

## 文件开头预览

```ps1
# PowerShell that uses [Wildcard] globbing and avoids the Set-Location issue.
$root = 'C:\Users\Administrator\Desktop\chenggong-jiachi-master\问题一\runs\2026-09-23-cache-test-rerun\snapshots'

# Use Get-ChildItem with -LiteralPath so PowerShell does not try to expand wildcards.
$dirs = Get-ChildItem -LiteralPath $root -Directory
foreach ($d in $dirs) {
    Write-Host ("--- " + $d.Name + " ---")
    $files = Get-ChildItem -LiteralPath $d.FullName -Filter 'call-*-response.json' | Sort-Object Name
    $total = 0; $none = 0; $score = 0; $valid = 0; $other = 0
    $unknowns = @()
    foreach ($f in $files) {
        $total++
        $j = Get-Content -LiteralPath $f.FullName -Raw | ConvertFrom-Json
        $t = $j.response.text
        if ($t -eq 'NONE') { $none++ }
        elseif ($t -match '】\s*\d+\s*$' -and $t -notmatch '】\s*\d+\s*【') { $score++ }
        elseif ($t.StartsWith('【【')) { $valid++ }
        else {
            $other++
            $unknowns += ($f.Name + ' :: ' + $t.Substring(0, [Math]::Min(60, $t.Length)))
        }
    }
    Write-Host ("Total=" + $total + " NONE=" + $none + " Score=" + $score + " Valid=" + $valid + " Other=" + $other)
    foreach ($u in $unknowns) { Write-Host ("  " + $u) }
}

```
