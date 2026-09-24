# debug6.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\debug6.ps1`  
> **分类**: 脚本  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T12:04:37.931Z  

## 文件开头预览

```ps1
$j = Get-Content 'reasoning-output-Z2-Q2.json' -Raw -Encoding UTF8 | ConvertFrom-Json
$l24 = [string]$j.llmOutput
$l24Len = $l24.Length

# Step A: Build lineStarts
$lineStarts = New-Object System.Collections.Generic.List[int]
$lineStarts.Add(0)
for ($i = 0; $i -lt $l24Len; $i++) {
    if ($l24[$i] -eq [char]10) { $lineStarts.Add($i + 1) }
}
Write-Output ("lineStarts count: " + $lineStarts.Count)

# Step B: Count lines starting with #
$hashedLines = 0
foreach ($ls in $lineStarts) {
    if ($ls -lt $l24Len -and $l24[$ls] -eq '#') { $hashedLines++ }
}
Write-Output ("Lines starting with #: " + $hashedLines)

# Step C: Try path detection
$LU = [char]0x8DEF
$JING = [char]0x5F84
$pathCount = 0
foreach ($ls in $lineStarts) {
    if ($ls -ge $l24Len) { continue }
    if ($l24[$ls] -ne '#') { continue }
    # get line
    $nextNL = $l24Len
    for ($ni = $ls + 1; $ni -lt $l24Len; $ni++) {
        if ($l24[$ni] -eq [char]10) { $nextNL = $ni; break }
    }
    $line = $l24.Substring($ls, $nextNL - $ls)
    # check for LU and JING
    $hasLu = $false
    $hasJing = $false
    for ($ci = 0; $ci -lt $line.Length; $ci++) {
        if ($line[$ci] -eq $LU) { $hasLu = $true }
        if ($line[$ci] -eq $JING) { $hasJing = $true }
    }
    if ($hasLu -and $hasJing) {
        $pathCount++
        Write-Output ("Path found at " + $ls + ": " + $line.Substring(0, [Math]::Min(40, $line.Length)))
    }
}
Write-Output ("Paths detected: " + $pathCount)

```
