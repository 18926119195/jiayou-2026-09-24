# extract_chunks2.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\extract_chunks2.ps1`  
> **分类**: 脚本  
> **大小**: 1.7 KB  
> **最后修改**: 2026-09-24T09:18:55.111Z  

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
    $startPos = $allMarkers[$i].pos + $allMarkers[$i].mlen
    if ($i -lt $allMarkers.Count - 1) { $endPos = $allMarkers[$i + 1].pos } else { $endPos = $line23.Length }
    $chunkText = $line23.Substring($startPos, $endPos - $startPos).Trim()
    $chunkText = $chunkText -replace "`n", " " -replace "`r", ""
    if ($chunkText.Length -gt 200) { $chunkText = $chunkText.Substring(0, 200) + " [..截断..]" }
    $allMarkers[$i].chunk = $chunkText
}

$regex24 = [regex]($LB + $LB + '(\d+)' + $RB + $RB)
$l24Numbers = @()
foreach ($m in $regex24.Matches($line24)) { $l24Numbers += $m.Groups[1].Value }

$lookup = @{}
foreach ($mkr in $allMarkers) {
    $n = $mkr.num
    if (-not $lookup.ContainsKey($n)) { $lookup[$n] = @() }
    $lookup[$n] += @{ pos = $mkr.pos; chunk = $mkr.chunk }
}

$count = 0
foreach ($n in $l24Numbers) {
    $count++
    $entries = $lookup[$n]
    if ($entries) {
        $tag = $LB + $LB + $n + $RB + $RB
        $header = "====== L24 REF#" + $count + ": " + $tag + " (L23 appears " + $entries.Count + "x) ======"
        Write-Host $header
        $idx = 1
        foreach ($e in $entries) {
            $clean = $e.chunk -replace '\s+', ' '
            Write-Host ("  [" + $idx + "] pos=" + $e.pos + ": " + $clean)
            $idx++
        }
        Write-Host ""
    }
```
