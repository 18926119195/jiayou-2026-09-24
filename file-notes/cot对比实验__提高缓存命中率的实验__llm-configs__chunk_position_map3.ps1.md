# chunk_position_map3.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\chunk_position_map3.ps1`  
> **分类**: 脚本  
> **大小**: 5.6 KB  
> **最后修改**: 2026-09-24T11:03:21.115Z  

## 文件开头预览

```ps1
$jsonData = ConvertFrom-Json ([System.IO.File]::ReadAllText('reasoning-output-Z1-Q4.json', [System.Text.Encoding]::UTF8))
$line23 = $jsonData.thinkingChain
$line24 = $jsonData.llmOutput

$sb = New-Object System.Text.StringBuilder
$sep = [string]::new([char]0x3D, 100)
$dash = [string]::new([char]0x2D, 60)

# Build regex using literal Chinese bracket chars concatenated into string
$LB = [string][char]0x3010  # 【
$RB = [string][char]0x3011  # 】
$singlePat = $LB + '(\d+)' + $RB
$doublePat = $LB + $LB + '(\d+)' + $RB + $RB

$singleRe = New-Object System.Text.RegularExpressions.Regex($singlePat)
$doubleRe = New-Object System.Text.RegularExpressions.Regex($doublePat)

Write-Host "singlePat bytes: $([System.Text.Encoding]::UTF8.GetBytes($singlePat) | ForEach-Object { $_.ToString('X2') })"
Write-Host "singleRe.IsNull: $($null -eq $singleRe)"
$test = 'hello 【123】 world'
$testMatches = $singleRe.Matches($test)
Write-Host "Test matches count: $($testMatches.Count)"
foreach ($tm in $testMatches) {
    Write-Host "  Match: $($tm.Value) at pos $($tm.Index), group1=$($tm.Groups[1].Value)"
}

function Get-All-Chunk-Positions([string]$text) {
    $results = @{}
    $matches = $script:singleRe.Matches($text)
    foreach ($m in $matches) {
        $n = $m.Groups[1].Value
        if (-not $results.ContainsKey($n)) { $results[$n] = New-Object System.Collections.Generic.List[int] }
        $results[$n].Add($m.Index)
    }
    return $results
}

function Get-L24-Path-Chunks([string]$text) {
    $lu = [string][char]0x8DEF
    $jing = [string][char]0x5F84
    $cnStr = ([string][char]0x4E00) + ([string][char]0x4E8C) + ([string][char]0x4E09) + ([string][char]0x56DB) + ([string][char]0x4E94) + ([string][char]0x516D) + ([string][char]0x4E03) + ([string][char]0x516B) + ([string][char]0x4E5D) + ([string][char]0x5341)
    $pathPat = '#\s*' + $lu + $jing + '[' + $cnStr + '][^#]*'
    $pathRe = New-Object System.Text.RegularExpressions.Regex($pathPat)

    $matches = $pathRe.Matches($text)
    $arr = New-Object 'System.Collections.Generic.List[object]'
    foreach ($m in $matches) {
        $block = $m.Value
        $newlineIdx = $block.IndexOf("`n")
        $title = if ($newlineIdx -gt 0) { $block.Substring(0, $newlineIdx).Trim() } else { $block.Substring(0, [Math]::Min(80, $block.Length)) }
```
