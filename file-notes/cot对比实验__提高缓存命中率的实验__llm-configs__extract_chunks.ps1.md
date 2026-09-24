# extract_chunks.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\extract_chunks.ps1`  
> **分类**: 脚本  
> **大小**: 2.6 KB  
> **最后修改**: 2026-09-24T09:17:37.505Z  

## 文件开头预览

```ps1
Set-Location -LiteralPath 'C:\Users\Administrator\Desktop\chenggong-jiachi-master\cot对比实验\提高缓存命中率的实验\llm-configs'
$content = [System.IO.File]::ReadAllText('reasoning-output-Z1-Q3.json', [System.Text.Encoding]::UTF8)
$lines = $content -split "`n"
$line23 = $lines[22]
$line24 = $lines[23]

$LB = [char]0x3010
$RB = [char]0x3011

# Step 1: Find ALL 【N】 positions in L23 with their following chunk content
# Chunk content = text after 【N】 until the next 【M】 marker (or end of line)
$allMarkers = @()
$regex = [regex]($LB + '(\d+)' + $RB)
foreach ($m in $regex.Matches($line23)) {
    $allMarkers += @{ num = $m.Groups[1].Value; pos = $m.Index; match = $m }
}

# Extract chunk content for each marker
for ($i = 0; $i -lt $allMarkers.Count; $i++) {
    $startPos = $allMarkers[$i].pos + $allMarkers[$i].match.Length
    if ($i -lt $allMarkers.Count - 1) {
        $endPos = $allMarkers[$i + 1].pos
    } else {
        $endPos = $line23.Length
    }
    $chunkText = $line23.Substring($startPos, $endPos - $startPos).Trim()
    $chunkText = $chunkText -replace "`n", " " -replace "`r", ""
    if ($chunkText.Length -gt 120) {
        $chunkText = $chunkText.Substring(0, 120) + "..."
    }
    $allMarkers[$i].chunk = $chunkText
}

# Step 2: Extract all 【【N】】 from L24 (in order of appearance)
$regex24 = [regex]($LB + $LB + '(\d+)' + $RB + $RB)
$l24Numbers = @()
foreach ($m in $regex24.Matches($line24)) {
    $l24Numbers += $m.Groups[1].Value
}

# Step 3: Build lookup: num -> array of (pos, chunk)
$lookup = @{}
foreach ($mkr in $allMarkers) {
    $n = $mkr.num
    if (-not $lookup.ContainsKey($n)) { $lookup[$n] = @() }
    $lookup[$n] += @{ pos = $mkr.pos; chunk = $mkr.chunk }
}

# Step 4: Output
Write-Host '=============================================================' -ForegroundColor Cyan
```
