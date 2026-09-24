# do_path_mapping3.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\do_path_mapping3.ps1`  
> **分类**: 脚本  
> **大小**: 5.0 KB  
> **最后修改**: 2026-09-24T10:26:35.928Z  

## 文件开头预览

```ps1
$content = [System.IO.File]::ReadAllText('reasoning-output-Z1-Q3.json', [System.Text.Encoding]::UTF8)
$lines = $content -split "`n"
$line24 = $lines[23]
$line23 = $lines[22]

$LB = [char]0x3010
$RB = [char]0x3011

$sb = New-Object System.Text.StringBuilder
$sep = [string]::new([char]0x3D, 78)
$dash = [string]::new([char]0x2D, 78)
$null = $sb.AppendLine($sep)
$null = $sb.AppendLine('L24 -> L23 PATH MAPPING')
$null = $sb.AppendLine($sep)

# Use Unicode range covering 一-十
$r24 = [regex]('#\s*\u8def\u5f84[\u4e00-\u56db]')
$h24 = @()
foreach ($m in $r24.Matches($line24)) {
    $cn = $m.Value.Trim().Substring($m.Value.Trim().Length - 1, 1)
    $h24 += @{n=$cn; p=$m.Index}
}
$h24 = @($h24 | Sort-Object p)

# Same for L23
$r23 = [regex]('#\s*\u8def\u5f84[\u4e00-\u56db]')
$h23 = @()
foreach ($m in $r23.Matches($line23)) {
    $cn = $m.Value.Trim().Substring($m.Value.Trim().Length - 1, 1)
    $h23 += @{n=$cn; p=$m.Index}
}
$h23 = @($h23 | Sort-Object p)

$null = $sb.AppendLine('L24 paths: ' + $h24.Count + ' | L23 paths: ' + $h23.Count)
$null = $sb.AppendLine('')

# Map chinese num -> arab
function Get-Arab([string]$cn) {
    switch -Regex ($cn) {
        '\u4e00' { return '1' }
        '\u4e8c' { return '2' }
        '\u4e09' { return '3' }
        '\u56db' { return '4' }
        '\u4e94' { return '5' }
        '\u516d' { return '6' }
        '\u4e03' { return '7' }
        '\u516b' { return '8' }
        '\u4e5d' { return '9' }
        '\u5341' { return '10' }
        default { return '?' }
```
