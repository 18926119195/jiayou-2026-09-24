# compare_ref4_ref24.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\compare_ref4_ref24.ps1`  
> **分类**: 脚本  
> **大小**: 2.9 KB  
> **最后修改**: 2026-09-24T09:40:51.528Z  

## 文件开头预览

```ps1
$content = [System.IO.File]::ReadAllText('reasoning-output-Z1-Q3.json', [System.Text.Encoding]::UTF8)
$lines = $content -split "`n"
$line23 = $lines[22]
$line24 = $lines[23]

$LB = [char]0x3010
$RB = [char]0x3011

$regex23 = [regex]($LB + '(\d+)' + $RB)
$allMarkers = @()
foreach ($m in $regex23.Matches($line23)) {
    $allMarkers += @{ num = $m.Groups[1].Value; pos = $m.Index; mlen = $m.Length }
}

for ($i = 0; $i -lt $allMarkers.Count; $i++) {
    if ($i -gt 0) { $startPos = $allMarkers[$i-1].pos + $allMarkers[$i-1].mlen } else { $startPos = 0 }
    $endPos = $allMarkers[$i].pos
    $beforeText = $line23.Substring($startPos, $endPos - $startPos).Trim()
    $beforeText = $beforeText -replace "`n", " " -replace "`r", ""
    if ($beforeText.Length -gt 400) { $beforeText = $beforeText.Substring($beforeText.Length - 400) }
    $beforeText = "..." + $beforeText
    $allMarkers[$i] | Add-Member -NotePropertyName "before" -NotePropertyValue $beforeText
}

$regex24 = [regex]($LB + $LB + '(\d+)' + $RB + $RB)
$l24Numbers = @()
foreach ($m in $regex24.Matches($line24)) { $l24Numbers += $m.Groups[1].Value }

$lookup = @{}
foreach ($mkr in $allMarkers) {
    $n = $mkr.num
    if (-not $lookup.ContainsKey($n)) { $lookup[$n] = @() }
    $lookup[$n] += $mkr.before
}

# Find the L24 positions of [[224]] in REF#4 and REF#24
$refCount = 0
$ref4Idx = $null
$ref24Idx = $null
foreach ($n in $l24Numbers) {
    $refCount++
    if ($refCount -eq 4) { $ref4Idx = $refCount }
    if ($refCount -eq 24) { $ref24Idx = $refCount }
}

$tag = "[[224]]"
$entries = $lookup["224"]

$sb = New-Object System.Text.StringBuilder
$null = $sb.AppendLine("============================================================")
```
