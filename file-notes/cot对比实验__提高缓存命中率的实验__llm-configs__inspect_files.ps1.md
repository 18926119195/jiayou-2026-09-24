# inspect_files.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\inspect_files.ps1`  
> **分类**: 脚本  
> **大小**: 1.8 KB  
> **最后修改**: 2026-09-24T11:50:13.508Z  

## 文件开头预览

```ps1
$ErrorActionPreference = 'Stop'

$files = @('reasoning-output-Z2-Q2.json','reasoning-output-Z2-Q3.json','reasoning-output-Z2-Q4.json','reasoning-output-Z3-Q3.json','reasoning-output-Z4-Q3.json')

Write-Host ("=" * 80)
Write-Host "FILE INSPECTION SUMMARY"
Write-Host ("=" * 80)

foreach ($f in $files) {
    if (Test-Path $f) {
        $raw = [System.IO.File]::ReadAllText($f, [System.Text.Encoding]::UTF8)
        $data = $raw | ConvertFrom-Json
        $l23 = [string]$data.thinkingChain
        $l24 = [string]$data.llmOutput
        $l23MentionCount = ([regex]::Matches($l23, [string][char]0x3010 + '(\d+)' + [string][char]0x3011)).Count
        $l23Unique = ([regex]::Matches($l23, [string][char]0x3010 + '(\d+)' + [string][char]0x3011) |
            ForEach-Object { $_.Groups[1].Value } | Sort-Object -Unique).Count
        $l24ChunkCount = ([regex]::Matches($l24, [string][char]0x3010 + [string][char]0x3010 + '(\d+)' + [string][char]0x3011 + [string][char]0x3011)).Count
        $l24Unique = ([regex]::Matches($l24, [string][char]0x3010 + [string][char]0x3010 + '(\d+)' + [string][char]0x3011 + [string][char]0x3011) |
            ForEach-Object { $_.Groups[1].Value } | Sort-Object -Unique).Count
        $paths = ([regex]::Matches($l24, '#\s*' + [string][char]0x8DEF + [string][char]0x5F84 + '[一二三四五六七八九十]+')).Count

        Write-Host ""
        Write-Host $f
        Write-Host ("  L23 chars:        {0}" -f $l23.Length)
        Write-Host ("  L24 chars:        {0}" -f $l24.Length)
        Write-Host ("  L23 mentions:     {0}  (unique: {1})" -f $l23MentionCount, $l23Unique)
        Write-Host ("  L24 chunks:       {0}  (unique: {1})" -f $l24ChunkCount, $l24Unique)
        Write-Host ("  L24 paths count:  {0}" -f $paths)
    } else {
        Write-Host ""
        Write-Host "$f : NOT FOUND"
    }
}

```
