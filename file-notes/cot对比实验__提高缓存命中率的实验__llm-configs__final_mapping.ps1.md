# final_mapping.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\final_mapping.ps1`  
> **分类**: 脚本  
> **大小**: 6.2 KB  
> **最后修改**: 2026-09-24T10:28:38.030Z  

## 文件开头预览

```ps1
$jsonData = ConvertFrom-Json ([System.IO.File]::ReadAllText('reasoning-output-Z1-Q3.json', [System.Text.Encoding]::UTF8))
$line24 = $jsonData.llmOutput
$line23 = $jsonData.thinkingChain

$LB = [char]0x3010
$RB = [char]0x3011

$sb = New-Object System.Text.StringBuilder
$sep = [string]::new([char]0x3D, 78)
$dash = [string]::new([char]0x2D, 78)

$null = $sb.AppendLine($sep)
$null = $sb.AppendLine('FINAL L24 -> L23 PATH MAPPING')
$null = $sb.AppendLine($sep)
$null = $sb.AppendLine('L23 (thinking) length: ' + $line23.Length + ' chars')
$null = $sb.AppendLine('L24 (output) length: ' + $line24.Length + ' chars')

# Build pattern with explicit chars
$lu = [string][char]0x8DEF
$jing = [string][char]0x5F84
$cnStr = ([string][char]0x4E00) + ([string][char]0x4E8C) + ([string][char]0x4E09) + ([string][char]0x56DB) + ([string][char]0x4E94) + ([string][char]0x516D) + ([string][char]0x4E03) + ([string][char]0x516B) + ([string][char]0x4E5D) + ([string][char]0x5341)

$pathPat = '#\s*' + $lu + $jing + '[' + $cnStr + ']'
$pathRe = [regex]($pathPat)

$chunkPat = $LB + $LB + '(\d+)' + $RB + $RB
$chunkRe = [regex]($chunkPat)

function Get-Arab([string]$cn) {
    $ord = [int][char]$cn
    switch ($ord) {
        0x4E00 { return '1' }
        0x4E8C { return '2' }
        0x4E09 { return '3' }
        0x56DB { return '4' }
        0x4E94 { return '5' }
        0x516D { return '6' }
        0x4E03 { return '7' }
        0x516B { return '8' }
        0x4E5D { return '9' }
        0x5341 { return '10' }
        default { return '?' }
    }
}

# Parse paths
$h24 = @()
foreach ($m in $pathRe.Matches($line24)) {
    $cn = $m.Value.Trim().Substring($m.Value.Trim().Length - 1, 1)
    $h24 += @{n=$cn; p=$m.Index}
```
