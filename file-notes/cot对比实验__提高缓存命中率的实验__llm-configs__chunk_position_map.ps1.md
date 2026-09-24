# chunk_position_map.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\chunk_position_map.ps1`  
> **分类**: 脚本  
> **大小**: 5.1 KB  
> **最后修改**: 2026-09-24T11:01:21.933Z  

## 文件开头预览

```ps1
$jsonData = ConvertFrom-Json ([System.IO.File]::ReadAllText('reasoning-output-Z1-Q4.json', [System.Text.Encoding]::UTF8))
$line23 = $jsonData.thinkingChain
$line24 = $jsonData.llmOutput

$sb = New-Object System.Text.StringBuilder
$sep = [string]::new([char]0x3D, 100)
$dash = [string]::new([char]0x2D, 60)

$LB = [char]0x3010
$RB = [char]0x3011

# Regex for both single-bracket 【N】 and double-bracket 【【N】】
$singleRe = New-Object System.Text.RegularExpressions.Regex('\[(\d+)\]')
$doubleRe = New-Object System.Text.RegularExpressions.Regex('\[\[(\d+)\]\]')

# Find all chunk mentions in L23 (both single and double bracket)
function Get-All-Chunk-Positions([string]$text) {
    $results = @{}
    foreach ($m in $singleRe.Matches($text)) {
        $n = $m.Groups[1].Value
        if (-not $results.ContainsKey($n)) { $results[$n] = New-Object System.Collections.Generic.List[int] }
        $results[$n].Add($m.Index)
    }
    return $results
}

# Extract L24 path -> chunks mapping
function Get-L24-Path-Chunks([string]$text) {
    $lu = [string][char]0x8DEF
    $jing = [string][char]0x5F84
    $cnStr = ([string][char]0x4E00) + ([string][char]0x4E8C) + ([string][char]0x4E09) + ([string][char]0x56DB) + ([string][char]0x4E94) + ([string][char]0x516D) + ([string][char]0x4E03) + ([string][char]0x516B) + ([string][char]0x4E5D) + ([string][char]0x5341)
    $pathRe = New-Object System.Text.RegularExpressions.Regex('#\s*' + $lu + $jing + '[' + $cnStr + '][^#]*')

    $matches = $pathRe.Matches($text)
    $arr = New-Object 'System.Collections.Generic.List[object]'
    foreach ($m in $matches) {
        $block = $m.Value
        $newlineIdx = $block.IndexOf("`n")
        $title = if ($newlineIdx -gt 0) { $block.Substring(0, $newlineIdx).Trim() } else { $block.Substring(0, [Math]::Min(80, $block.Length)) }
        $chunks = @()
        foreach ($cm in $doubleRe.Matches($block)) { $chunks += $cm.Groups[1].Value }
        $uniqueChunks = ($chunks | Sort-Object -Unique)
        $arr.Add(@{ title = $title; chunks = $uniqueChunks; block = $block })
    }
    return $arr
}

$paths24 = Get-L24-Path-Chunks $line24
$chunkPositions = Get-All-Chunk-Positions $line23

```
