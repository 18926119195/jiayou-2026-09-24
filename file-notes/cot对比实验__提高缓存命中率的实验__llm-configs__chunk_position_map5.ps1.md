# chunk_position_map5.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\chunk_position_map5.ps1`  
> **分类**: 脚本  
> **大小**: 6.4 KB  
> **最后修改**: 2026-09-24T11:05:29.595Z  

## 文件开头预览

```ps1
$ErrorActionPreference = 'Stop'

$jsonData = ConvertFrom-Json ([System.IO.File]::ReadAllText('reasoning-output-Z1-Q4.json', [System.Text.Encoding]::UTF8))
$line23 = [string]$jsonData.thinkingChain
$line24 = [string]$jsonData.llmOutput

$sb = New-Object System.Text.StringBuilder
$sep = [string]::new([char]0x3D, 80)
$dash = [string]::new([char]0x2D, 60)

$LB = [string][char]0x3010  # 【
$RB = [string][char]0x3011  # 】

# Use [char] cast inside the pattern to avoid issues
$singlePat = [string]$LB + '(\d+)' + [string]$RB
$doublePat = [string]$LB + [string]$LB + '(\d+)' + [string]$RB + [string]$RB

# Use the static Regex.Match / Regex.Matches method directly
$test = 'hello ' + $LB + '123' + $RB + ' world'
$testMatches = [System.Text.RegularExpressions.Regex]::Matches($test, $singlePat)
Write-Host "Test pattern length: $($singlePat.Length)"
Write-Host "Test matches count: $($testMatches.Count)"

# Find all chunk positions in L23
$chunkPositions = @{}
$matches23 = [System.Text.RegularExpressions.Regex]::Matches($line23, $singlePat)
Write-Host "L23 single-bracket matches: $($matches23.Count)"

foreach ($m in $matches23) {
    $n = $m.Groups[1].Value
    if (-not $chunkPositions.ContainsKey($n)) {
        $chunkPositions[$n] = New-Object System.Collections.Generic.List[int]
    }
    $chunkPositions[$n].Add($m.Index)
}

# Extract L24 paths and chunks
$lu = [string][char]0x8DEF
$jing = [string][char]0x5F84
$cnStr = ([string][char]0x4E00) + ([string][char]0x4E8C) + ([string][char]0x4E09) + ([string][char]0x56DB) + ([string][char]0x4E94) + ([string][char]0x516D) + ([string][char]0x4E03) + ([string][char]0x516B) + ([string][char]0x4E5D) + ([string][char]0x5341)
$pathPat = '#\s*' + $lu + $jing + '[' + $cnStr + '][^#]*'
$pathMatches = [System.Text.RegularExpressions.Regex]::Matches($line24, $pathPat)

$paths24 = New-Object 'System.Collections.Generic.List[object]'
foreach ($m in $pathMatches) {
    $block = $m.Value
    $newlineIdx = $block.IndexOf("`n")
    $title = if ($newlineIdx -gt 0) { $block.Substring(0, $newlineIdx).Trim() } else { $block.Substring(0, [Math]::Min(80, $block.Length)) }
    $chunks = @()
    $chunkMatches = [System.Text.RegularExpressions.Regex]::Matches($block, $doublePat)
```
