# debug_pat.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\debug_pat.ps1`  
> **分类**: 脚本  
> **大小**: 2.1 KB  
> **最后修改**: 2026-09-24T10:23:16.530Z  

## 文件开头预览

```ps1
$content = [System.IO.File]::ReadAllText('reasoning-output-Z1-Q3.json', [System.Text.Encoding]::UTF8)
$lines = $content -split "`n"
$line24 = $lines[23]
$line23 = $lines[22]

$sb = New-Object System.Text.StringBuilder
$null = $sb.AppendLine('L24 length: ' + $line24.Length)
$null = $sb.AppendLine('L23 length: ' + $line23.Length)

# Build chars one by one  
$cn1 = [string][char]0x4E00
$cn2 = [string][char]0x4E8C
$cn3 = [string][char]0x4E09
$cn4 = [string][char]0x56DB
$cn5 = [string][char]0x4E94
$cn6 = [string][char]0x516D
$cn7 = [string][char]0x4E03
$cn8 = [string][char]0x516B
$cn9 = [string][char]0x4E5D
$cn10 = [string][char]0x5341
$lu = [string][char]0x8DEF
$jing = [string][char]0x5F84
$colon = [string][char]0xFF1A

$null = $sb.AppendLine('chars: ' + $cn1 + $cn2 + $cn3 + $cn4 + $cn5 + $cn6 + $cn7 + $cn8 + $cn9 + $cn10 + $colon)
$null = $sb.AppendLine('pat test: #' + $lu + $jing + ' ' + $cn1 + $colon)
$null = $sb.AppendLine('L24[0..100]: ' + $line24.Substring(0, 80))

# Build pattern as string
$cnChars = [string]$cn1 + [string]$cn2 + [string]$cn3 + [string]$cn4 + [string]$cn5 + [string]$cn6 + [string]$cn7 + [string]$cn8 + [string]$cn9 + [string]$cn10
$pat = '#' + $lu + $jing + '([' + $cnChars + '])' + $colon
$null = $sb.AppendLine('REGEX pattern (escaped): ' + ($pat -replace '\\', '\\\\'))
$null = $sb.AppendLine('REGEX pattern (raw): ' + $pat)

# Test the regex
$r24 = [regex]$pat
$null = $sb.AppendLine('r24.IsMatch(line24): ' + $r24.IsMatch($line24))
$ms = $r24.Matches($line24)
$null = $sb.AppendLine('Number of matches: ' + $ms.Count)
foreach ($m in $ms) {
    $null = $sb.AppendLine('  Match @ ' + $m.Index + ': ' + $m.Value + ' [group1=' + $m.Groups[1].Value + ']')
}

# Try simpler regex
$rSimple = [regex]('#\s*\u8def\u5f84[\u4e00-\u5341]')
$null = $sb.AppendLine('')
$null = $sb.AppendLine('Try Unicode escapes:')
$ms2 = $rSimple.Matches($line24)
$null = $sb.AppendLine('Simple pattern matches: ' + $ms2.Count)
foreach ($m in $ms2) {
```
