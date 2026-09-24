# verify_paths.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\verify_paths.ps1`  
> **分类**: 脚本  
> **大小**: 5.1 KB  
> **最后修改**: 2026-09-24T09:57:10.037Z  

## 文件开头预览

```ps1
﻿$content = [System.IO.File]::ReadAllText('reasoning-output-Z1-Q3.json', [System.Text.Encoding]::UTF8)
$lines = $content -split "`n"
$line23 = $lines[22]
$line24 = $lines[23]

$sep = '=' * 70

$sb = New-Object System.Text.StringBuilder

$null = $sb.AppendLine($sep)
$null = $sb.AppendLine('L23 PATH MARKERS')
$null = $sb.AppendLine($sep)

# English: "Path N" 
$regexEn = [regex]'(?i)\bpath\s*(\d+)\b'
$pathsEn = @()
foreach ($m in $regexEn.Matches($line23)) {
    $n = $m.Groups[1].Value
    $pos = $m.Index
    $ctx = $line23.Substring([Math]::Max(0,$pos-30), [Math]::Min(100, $line23.Length-$pos+30))
    $ctx = $ctx -replace "`n", ' ' -replace "`r", ''
    $pathsEn += @{ num = $n; pos = $pos; ctx = $ctx }
}

# Chinese: "lu jing" (path) + chinese number 
$zhMap = @{ [char]0x4E00='1'; [char]0x4E8C='2'; [char]0x4E09='3'; [char]0x56DB='4'; [char]0x4E94='5'; [char]0x516D='6'; [char]0x4E03='7'; [char]0x516B='8'; [char]0x4E5D='9'; [char]0x5341='10' }
$regexZh = New-Object System.Text.RegularExpressions.Regex([string]::Format([char]0x8DEF + [char]0x5F84 + '\s*([{0}{1}{2}{3}{4}{5}{6}{7}{8}{9}])\s*[{10}{11}]', [char]0x4E00, [char]0x4E8C, [char]0x4E09, [char]0x56DB, [char]0x4E94, [char]0x516D, [char]0x4E03, [char]0x516B, [char]0x4E5D, [char]0x5341, [char]0xFF1A, [char]0x003A))
$pathsZh = @()
foreach ($m in $regexZh.Matches($line23)) {
    $cn = $m.Groups[1].Value
    $n = $zhMap[$cn]
    if (-not $n) { $n = '?' }
    $pos = $m.Index
    $ctx = $line23.Substring([Math]::Max(0,$pos-30), [Math]::Min(100, $line23.Length-$pos+30))
    $ctx = $ctx -replace "`n", ' ' -replace "`r", ''
    $pathsZh += @{ num = $n; cn = $cn; pos = $pos; ctx = $ctx }
}

# Step markers
$regexStep = New-Object System.Text.RegularExpressions.Regex([string]::Format('(?:step|{0}{1}{2})\s*(\d+)\s*[{3}{4}]', [char]0x6B65, [char]0x9AA4, [char]0x3001, [char]0xFF1A, [char]0x003A))
$stepsEn = @()
foreach ($m in $regexStep.Matches($line23)) {
    $stepsEn += @{ num = $m.Groups[1].Value; pos = $m.Index }
}

$null = $sb.AppendLine('English Path markers: ' + $pathsEn.Count)
foreach ($p in $pathsEn) {
    $null = $sb.AppendLine('  Path ' + $p.num + ' @ ' + $p.pos + ': ' + $p.ctx)
}
$null = $sb.AppendLine('')
```
