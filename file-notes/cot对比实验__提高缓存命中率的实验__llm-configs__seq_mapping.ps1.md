# seq_mapping.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\seq_mapping.ps1`  
> **分类**: 脚本  
> **大小**: 3.2 KB  
> **最后修改**: 2026-09-24T09:49:56.048Z  

## 文件开头预览

```ps1
$content = [System.IO.File]::ReadAllText('reasoning-output-Z1-Q3.json', [System.Text.Encoding]::UTF8)
$lines = $content -split "`n"
$line23 = $lines[22]
$line24 = $lines[23]

$LB = [char]0x3010
$RB = [char]0x3011

# L23: single 【N】, extract (pos, num, beforeText, afterText)
$regex23 = [regex]($LB + '(\d+)' + $RB)
$l23Items = @()
foreach ($m in $regex23.Matches($line23)) {
    $num = $m.Groups[1].Value
    $pos = $m.Index
    $mlen = $m.Length
    # afterText = the marker itself + next 200 chars
    $end = [Math]::Min($line23.Length, $pos + $mlen + 200)
    $afterText = $line23.Substring($pos + $mlen, $end - $pos - $mlen).Trim()
    $afterText = $afterText -replace "`n", " " -replace "`r", ""
    if ($afterText.Length -gt 200) { $afterText = $afterText.Substring(0, 200) + "..." }
    # beforeText = 400 chars before marker
    $start = [Math]::Max(0, $pos - 400)
    $beforeText = $line23.Substring($start, $pos - $start).Trim()
    $beforeText = $beforeText -replace "`n", " " -replace "`r", ""
    if ($beforeText.Length -gt 400) { $beforeText = "..." + $beforeText.Substring($beforeText.Length - 400) }
    $l23Items += @{
        idx = $l23Items.Count + 1
        num = $num
        pos = $pos
        beforeText = $beforeText
        afterText = $afterText
    }
}

# L24: double 【【N】】, extract (pos, num, afterText)
$regex24 = [regex]($LB + $LB + '(\d+)' + $RB + $RB)
$l24Items = @()
foreach ($m in $regex24.Matches($line24)) {
    $num = $m.Groups[1].Value
    $pos = $m.Index
    $mlen = $m.Length
    $end = [Math]::Min($line24.Length, $pos + $mlen + 200)
    $afterText = $line24.Substring($pos + $mlen, $end - $pos - $mlen).Trim()
    $afterText = $afterText -replace "`n", " " -replace "`r", ""
    if ($afterText.Length -gt 200) { $afterText = $afterText.Substring(0, 200) + "..." }
    $l24Items += @{
        idx = $l24Items.Count + 1
        num = $num
        pos = $pos
        afterText = $afterText
```
