# chunk_position_z2q2.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\chunk_position_z2q2.ps1`  
> **分类**: 脚本  
> **大小**: 6.8 KB  
> **最后修改**: 2026-09-24T11:15:27.188Z  

## 文件开头预览

```ps1
$ErrorActionPreference = 'Stop'

$jsonData = ConvertFrom-Json ([System.IO.File]::ReadAllText('reasoning-output-Z2-Q2.json', [System.Text.Encoding]::UTF8))
$line23 = [string]$jsonData.thinkingChain
$line24 = [string]$jsonData.llmOutput

$sb = New-Object System.Text.StringBuilder
$sep = [string]::new([char]0x3D, 80)
$dash = [string]::new([char]0x2D, 60)

$LB = [string][char]0x3010
$RB = [string][char]0x3011
$singlePat = [string]$LB + '(\d+)' + [string]$RB
$doublePat = [string]$LB + [string]$LB + '(\d+)' + [string]$RB + [string]$RB

# Find all chunk positions in L23
$matches23 = [System.Text.RegularExpressions.Regex]::Matches($line23, $singlePat)
$chunkPositions = @{}
foreach ($m in $matches23) {
    $n = $m.Groups[1].Value
    if (-not $chunkPositions.ContainsKey($n)) {
        $chunkPositions[$n] = New-Object System.Collections.Generic.List[int]
    }
    $chunkPositions[$n].Add($m.Index)
}

# Extract L24 paths
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
    foreach ($cm in $chunkMatches) { $chunks += $cm.Groups[1].Value }
    $uniqueChunks = ($chunks | Sort-Object -Unique)
    $paths24.Add(@{ title = $title; chunks = $uniqueChunks })
}

$null = $sb.AppendLine($sep)
$null = $sb.AppendLine('Z2-Q2: CHUNK-BASED POSITION MAPPING')
$null = $sb.AppendLine($sep)
$null = $sb.AppendLine('')
$null = $sb.AppendLine('L23 length: ' + $line23.Length)
```
