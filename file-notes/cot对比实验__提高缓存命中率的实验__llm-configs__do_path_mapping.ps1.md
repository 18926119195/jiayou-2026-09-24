# do_path_mapping.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\do_path_mapping.ps1`  
> **分类**: 脚本  
> **大小**: 4.6 KB  
> **最后修改**: 2026-09-24T10:05:38.424Z  

## 文件开头预览

```ps1
$content = [System.IO.File]::ReadAllText('reasoning-output-Z1-Q3.json', [System.Text.Encoding]::UTF8)
$lines = $content -split "`n"
$line23 = $lines[22]
$line24 = $lines[23]

$cLB = [char]0x3010  # [
$cRB = [char]0x3011  # ]
$cHua = [char]0x300A  # 《
$cHua2 = [char]0x300B # 》
$c1 = [char]0x4E00; $c2 = [char]0x4E8C; $c3 = [char]0x4E09; $c4 = [char]0x56DB
$c5 = [char]0x4E94; $c6 = [char]0x516D; $c7 = [char]0x4E03; $c8 = [char]0x516B
$c9 = [char]0x4E5D; $c10 = [char]0x5341
$cColon = [char]0xFF1A
$cSlash = [char]0x002F

$zhToArab = @{}
$zhToArab[$c1]='1'; $zhToArab[$c2]='2'; $zhToArab[$c3]='3'; $zhToArab[$c4]='4'
$zhToArab[$c5]='5'; $zhToArab[$c6]='6'; $zhToArab[$c7]='7'; $zhToArab[$c8]='8'
$zhToArab[$c9]='9'; $zhToArab[$c10]='10'

# L24 path pattern
$pat24 = '(?s)#\s*路径([' + $c1 + $c2 + $c3 + $c4 + $c5 + $c6 + $c7 + $c8 + $c9 + $c10 + '])' + $cColon + '(.+?)(?=\n---+|\n#\s*路径|\Z)'
$r24 = New-Object System.Text.RegularExpressions.Regex($pat24)
$pathBlocks24 = @()
foreach ($m in $r24.Matches($line24)) {
    $title = $m.Groups[2].Value.Trim()
    $full = $m.Value
    $chunks = @()
    $cr = New-Object System.Text.RegularExpressions.Regex('\[\[(\d+)\]\]')
    foreach ($cm in $cr.Matches($full)) { $chunks += $cm.Groups[1].Value }
    $pathBlocks24 += @{title=$title; full=$full; chunks=$chunks}
}

# L23 path pattern
$pat23 = '(?s)#\s*路径([' + $c1 + $c2 + $c3 + $c4 + $c5 + $c6 + $c7 + $c8 + $c9 + $c10 + '])' + $cColon
$r23 = New-Object System.Text.RegularExpressions.Regex($pat23)
$ph23 = @()
foreach ($m in $r23.Matches($line23)) {
    $ph23 += @{pathNum=$m.Groups[1].Value; pos=$m.Index}
}
$ph23 = @($ph23 | Sort-Object pos)
for ($i = 0; $i -lt $ph23.Count; $i++) {
    $s = $ph23[$i].pos
    $e = if ($i+1 -lt $ph23.Count) { $ph23[$i+1].pos } else { $line23.Length }
    $ph23[$i].start=$s; $ph23[$i].end=$e
    $ph23[$i].content=$line23.Substring($s, $e-$s)
}

function Get-Sim($a, $b) {
    $ca = $a.ToCharArray(); $cb = $b.ToCharArray()
```
