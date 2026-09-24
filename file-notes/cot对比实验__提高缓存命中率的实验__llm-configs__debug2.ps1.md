# debug2.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\debug2.ps1`  
> **分类**: 脚本  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T11:59:01.491Z  

## 文件开头预览

```ps1
$raw = [System.IO.File]::ReadAllText("reasoning-output-Z2-Q2.json", [System.Text.Encoding]::UTF8)
$data = $raw | ConvertFrom-Json
$l24 = [string]$data.llmOutput
$l24Len = $l24.Length
Write-Host "L24 length: $l24Len"

$lineStarts = @(0)
for ($i = 0; $i -lt $l24Len; $i++) {
    if ($l24[$i] -eq "`n") { $lineStarts += ($i + 1) }
}
Write-Host "Line starts count: $($lineStarts.Count)"
Write-Host "First 5 line starts: $($lineStarts[0..[Math]::Min(4,$lineStarts.Count-1)] -join ', ')"

$lu = [char]0x8DEF
$jing = [char]0x5F84
$CN_NUMS = "一二三四五六七八九十"
$paths = 0

for ($li = 0; $li -lt $lineStarts.Count; $li++) {
    $ls = $lineStarts[$li]
    if ($ls -ge $l24Len) { continue }
    $ch = $l24[$ls]
    if ($ch -eq '#') {
        $nextNL = $l24.IndexOf("`n", $ls)
        if ($nextNL -lt 0) { $nextNL = $l24Len }
        $line = $l24.Substring($ls, $nextNL - $ls)
        $hasLu = $line.IndexOf($lu) -ge 0
        $hasJing = $line.IndexOf($jing) -ge 0
        if ($hasLu -and $hasJing) {
            $paths++
            Write-Host "Path found at line start $ls: $($line.Substring(0, [Math]::Min(60, $line.Length)))"
        }
    }
}
Write-Host "Total paths found: $paths"

# Also try without the lu/jing check
$hashLines = 0
for ($li = 0; $li -lt $lineStarts.Count; $li++) {
    $ls = $lineStarts[$li]
    if ($ls -ge $l24Len) { continue }
    if ($l24[$ls] -eq '#') {
        $hashLines++
    }
}
Write-Host "Lines starting with #: $hashLines"

```
