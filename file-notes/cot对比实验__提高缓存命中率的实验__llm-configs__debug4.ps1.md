# debug4.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\debug4.ps1`  
> **分类**: 脚本  
> **大小**: 0.7 KB  
> **最后修改**: 2026-09-24T12:03:52.209Z  

## 文件开头预览

```ps1
$raw = [System.IO.File]::ReadAllText("reasoning-output-Z2-Q2.json", [System.Text.Encoding]::UTF8)
$data = $raw | ConvertFrom-Json
$l24 = [string]$data.llmOutput

$idx = $l24.IndexOf("#")
$lineEnd = $l24.IndexOf([char]10, $idx)
$line = $l24.Substring($idx, $lineEnd - $idx)

Write-Output ("First line: " + $line)
Write-Output ("Char codes after #:")
for ($i = 0; $i -lt [Math]::Min(15, $line.Length); $i++) {
    Write-Output ("[" + $i + "] code=" + [int]$line[$i] + " char=" + $line[$i])
}

# Search for codes 0x8DEF and 0x5F84
Write-Output "Search for 0x8DEF in line:"
for ($i = 0; $i -lt $line.Length; $i++) {
    if ([int]$line[$i] -eq 0x8DEF) {
        Write-Output ("Found at " + $i + " next char code=" + [int]$line[$i+1])
    }
}

```
