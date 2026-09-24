# extract_before2.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\extract_before2.ps1`  
> **分类**: 脚本  
> **大小**: 1.8 KB  
> **最后修改**: 2026-09-24T09:24:23.806Z  

## 文件开头预览

```ps1
$content = [System.IO.File]::ReadAllText('reasoning-output-Z1-Q3.json', [System.Text.Encoding]::UTF8)
$lines = $content -split "`n"
$line23 = $lines[22]
$line24 = $lines[23]

$LB = [char]0x3010
$RB = [char]0x3011

$regex = [regex]($LB + '(\d+)' + $RB)
$allMarkers = @()
foreach ($m in $regex.Matches($line23)) {
    $allMarkers += @{ num = $m.Groups[1].Value; pos = $m.Index; mlen = $m.Length }
}

for ($i = 0; $i -lt $allMarkers.Count; $i++) {
    if ($i -gt 0) { $startPos = $allMarkers[$i-1].pos + $allMarkers[$i-1].mlen } else { $startPos = 0 }
    $endPos = $allMarkers[$i].pos
    $beforeText = $line23.Substring($startPos, $endPos - $startPos).Trim()
    $beforeText = $beforeText -replace "`n", " " -replace "`r", ""
    if ($beforeText.Length -gt 300) { $beforeText = $beforeText.Substring($beforeText.Length - 300) }
    $beforeText = "..." + $beforeText
    $allMarkers[$i].before = $beforeText
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

$sb = New-Object System.Text.StringBuilder
$count = 0
foreach ($n in $l24Numbers) {
    $count++
    $entries = $lookup[$n]
    if ($entries) {
        $tag = "[[" + $n + "]]"
        $null = $sb.AppendLine("")
        $null = $sb.AppendLine("====== L24 REF# $count : $tag (L23中共有 $($entries.Count) 处引用) ======")
        $idx = 1
        foreach ($bt in $entries) {
            $clean = $bt -replace '\s+', ' '
            $null = $sb.AppendLine("  [$idx] $clean")
            $idx++
        }
```
