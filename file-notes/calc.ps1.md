# calc.ps1

> **路径**: `calc.ps1`  
> **分类**: 脚本  
> **大小**: 1.9 KB  
> **最后修改**: 2026-09-24T09:24:17.709Z  

## 文件开头预览

```ps1
$tokens = @(
  ,(160128, 215, 7233)
  ,(160128, 211, 6897)
  ,(160000, 338, 8298)
  ,(160000, 338, 13947)
  ,(160000, 345, 6692)
  ,(160000, 343, 12310)
  ,(160000, 350, 17283)
  ,(160000, 343, 9525)
  ,(160128, 222, 9981)
  ,(160128, 214, 13694)
  ,(160000, 342, 9655)
  ,(160000, 341, 16684)
  ,(160000, 345, 10616)
  ,(160000, 349, 8819)
  ,(160000, 342, 5508)
)
$qids = @('Z1-Q1','Z1-Q2','Z1-Q3','Z1-Q4','Z2-Q1','Z2-Q2','Z2-Q3','Z2-Q4','Z3-Q1','Z3-Q2','Z3-Q3','Z4-Q1','Z4-Q2','Z4-Q3','Z4-Q4')

Write-Host "=== PEAK pricing (h=0.006, m=0.30, o=1.20) ==="
$h = 0.006; $m = 0.30; $o = 1.20
$total = 0.0
for ($i = 0; $i -lt 15; $i++) {
  $ch = $tokens[$i][0]; $cm = $tokens[$i][1]; $ct = $tokens[$i][2]
  $cost = $ch/1e6*$h + $cm/1e6*$m + $ct/1e6*$o
  $total += $cost
  Write-Host "$($qids[$i]): $([math]::Round($cost,5)) USD  ($( [math]::Round($cost*7.2,3) ) CNY)"
}
Write-Host "Total USD: $([math]::Round($total,5))"
Write-Host "Total CNY @7.2: $([math]::Round($total*7.2,3))"
Write-Host "Total CNY @7.3: $([math]::Round($total*7.3,3))"

Write-Host ""
Write-Host "=== NON-PEAK pricing (h=0.003, m=0.15, o=0.60) ==="
$h = 0.003; $m = 0.15; $o = 0.60
$total2 = 0.0
for ($i = 0; $i -lt 15; $i++) {
  $ch = $tokens[$i][0]; $cm = $tokens[$i][1]; $ct = $tokens[$i][2]
  $cost = $ch/1e6*$h + $cm/1e6*$m + $ct/1e6*$o
  $total2 += $cost
  Write-Host "$($qids[$i]): $([math]::Round($cost,5)) USD  ($( [math]::Round($cost*7.2,3) ) CNY)"
}
Write-Host "Total USD: $([math]::Round($total2,5))"
Write-Host "Total CNY @7.2: $([math]::Round($total2*7.2,3))"
Write-Host "Total CNY @7.3: $([math]::Round($total2*7.3,3))"

Write-Host ""
Write-Host "=== Key totals ==="
$ch_t = ($tokens | ForEach-Object { $_[0] } | Measure-Object -Sum).Sum
$cm_t = ($tokens | ForEach-Object { $_[1] } | Measure-Object -Sum).Sum
```
