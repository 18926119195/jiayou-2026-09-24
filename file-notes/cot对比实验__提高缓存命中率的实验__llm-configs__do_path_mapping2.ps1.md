# do_path_mapping2.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\do_path_mapping2.ps1`  
> **分类**: 脚本  
> **大小**: 4.0 KB  
> **最后修改**: 2026-09-24T10:22:29.517Z  

## 文件开头预览

```ps1
$content = [System.IO.File]::ReadAllText('reasoning-output-Z1-Q3.json', [System.Text.Encoding]::UTF8)
$lines = $content -split "`n"
$line24 = $lines[23]
$line23 = $lines[22]

$LB = [char]0x3010
$RB = [char]0x3011

$sb = New-Object System.Text.StringBuilder
$null = $sb.AppendLine('L24 length: ' + $line24.Length)
$null = $sb.AppendLine('L23 length: ' + $line23.Length)

# Build chinese number chars
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

# L24: find each #\u8def\u5f84N:\u3011 header
$ZHNUMS = @{}
$ZHNUMS[$cn1]='1'; $ZHNUMS[$cn2]='2'; $ZHNUMS[$cn3]='3'; $ZHNUMS[$cn4]='4'
$ZHNUMS[$cn5]='5'; $ZHNUMS[$cn6]='6'; $ZHNUMS[$cn7]='7'; $ZHNUMS[$cn8]='8'
$ZHNUMS[$cn9]='9'; $ZHNUMS[$cn10]='10'

# Build the pattern
$cnChars = $cn1 + $cn2 + $cn3 + $cn4 + $cn5 + $cn6 + $cn7 + $cn8 + $cn9 + $cn10
$pat = '#\s*' + $lu + $jing + '([' + $cnChars + '])' + $colon
$r24 = [regex]$pat
$h24 = @()
foreach ($m in $r24.Matches($line24)) {
    $h24 += @{n=$m.Groups[1].Value; p=$m.Index}
}
$h24 = @($h24 | Sort-Object p)
$null = $sb.AppendLine('')
$null = $sb.AppendLine('L24 paths found: ' + $h24.Count)
for ($i = 0; $i -lt $h24.Count; $i++) {
    $start = $h24[$i].p
    $end = if ($i+1 -lt $h24.Count) { $h24[$i+1].p } else { $line24.Length }
    $h24[$i].start = $start
    $h24[$i].end = $end
    $h24[$i].block = $line24.Substring($start, $end - $start)
```
