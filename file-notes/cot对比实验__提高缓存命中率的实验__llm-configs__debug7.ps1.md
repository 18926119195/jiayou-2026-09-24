# debug7.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\debug7.ps1`  
> **分类**: 脚本  
> **大小**: 0.8 KB  
> **最后修改**: 2026-09-24T12:04:55.265Z  

## 文件开头预览

```ps1
$raw = [System.IO.File]::ReadAllText("reasoning-output-Z2-Q2.json", [System.Text.Encoding]::UTF8)
$data = $raw | ConvertFrom-Json
$l24 = [string]$data.llmOutput
$l24Len = $l24.Length
$NL = [char]10
$LU = [char]0x8DEF
$JING = [char]0x5F84

Write-Output ("NL code: " + [int]$NL)
Write-Output ("LU code: " + [int]$LU)
Write-Output ("JING code: " + [int]$JING)

# Check a sample char in l24
Write-Output ("l24[0] = '" + $l24[0] + "' code=" + [int]$l24[0])
Write-Output ("l24[1] = '" + $l24[1] + "' code=" + [int]$l24[1])
Write-Output ("l24[2] = '" + $l24[2] + "' code=" + [int]$l24[2])
Write-Output ("l24[3] = '" + $l24[3] + "' code=" + [int]$l24[3])

# Test equality
Write-Output ("l24[2] -eq LU: " + ($l24[2] -eq $LU))
Write-Output ("l24[2] -eq JING: " + ($l24[2] -eq $JING))
Write-Output ("l24[3] -eq JING: " + ($l24[3] -eq $JING))

```
