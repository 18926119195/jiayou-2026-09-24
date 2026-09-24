# demo_match.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\demo_match.ps1`  
> **分类**: 脚本  
> **大小**: 2.8 KB  
> **最后修改**: 2026-09-24T08:57:16.481Z  

## 文件开头预览

```ps1
Set-Location -LiteralPath 'C:\Users\Administrator\Desktop\chenggong-jiachi-master\cot对比实验\提高缓存命中率的实验\llm-configs'
$content = [System.IO.File]::ReadAllText('reasoning-output-Z1-Q3.json', [System.Text.Encoding]::UTF8)
$lines = $content -split "`n"
$line23 = $lines[22]
$line24 = $lines[23]

$LB = [char]0x3010
$RB = [char]0x3011

Write-Host '=== FILE STATS ===' -ForegroundColor Cyan
Write-Host ('L23 length: ' + $line23.Length + ' chars')
Write-Host ('L24 length: ' + $line24.Length + ' chars')
Write-Host ''

$pattern23 = $LB + '(\d+)' + $RB
$regex23 = [regex]$pattern23
$matches23 = $regex23.Matches($line23)
$nums23 = @()
foreach ($m in $matches23) { $nums23 += $m.Groups[1].Value }
$unique23 = $nums23 | Sort-Object -Unique

Write-Host '=== L23 (thinkingChain) ===' -ForegroundColor Cyan
Write-Host ('Total N matches: ' + $matches23.Count)
Write-Host ('Unique numbers (' + $unique23.Count + '): ' + ($unique23 -join ', '))
Write-Host ''

$pattern24 = $LB + $LB + '(\d+)' + $RB + $RB
$regex24 = [regex]$pattern24
$matches24 = $regex24.Matches($line24)
$nums24 = @()
foreach ($m in $matches24) { $nums24 += $m.Groups[1].Value }
$unique24 = $nums24 | Sort-Object -Unique

Write-Host '=== L24 (llmOutput) ===' -ForegroundColor Cyan
Write-Host ('Total N matches: ' + $matches24.Count)
Write-Host ('Unique numbers (' + $unique24.Count + '): ' + ($unique24 -join ', '))
Write-Host ''

$missingIn23 = $unique24 | Where-Object { $_ -notin $unique23 }
$extraIn23 = $unique23 | Where-Object { $_ -notin $unique24 }

Write-Host '=== DIFF ===' -ForegroundColor Yellow
if ($missingIn23.Count -eq 0) {
    Write-Host 'All L24 numbers found in L23 (no hallucinations)' -ForegroundColor Green
} else {
    Write-Host ('L24 not in L23: ' + ($missingIn23 -join ', ')) -ForegroundColor Red
}
Write-Host ('L23 dropped: ' + ($extraIn23 -join ', '))
Write-Host ''

```
