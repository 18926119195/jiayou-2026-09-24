# find_non_ascii.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\find_non_ascii.ps1`  
> **分类**: 脚本  
> **大小**: 0.3 KB  
> **最后修改**: 2026-09-24T12:00:30.077Z  

## 文件开头预览

```ps1
$content = Get-Content 'trace_mapper.ps1' -Encoding UTF8
$lineNum = 0
foreach ($line in $content) {
    $lineNum++
    if ($line -match '[^\x00-\x7F]') {
        Write-Host ("L$lineNum has non-ASCII: " + ($line.Substring(0, [Math]::Min(60, $line.Length))))
    }
}

```
