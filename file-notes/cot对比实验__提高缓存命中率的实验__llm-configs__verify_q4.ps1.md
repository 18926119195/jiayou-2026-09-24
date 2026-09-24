# verify_q4.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\verify_q4.ps1`  
> **分类**: 脚本  
> **大小**: 5.1 KB  
> **最后修改**: 2026-09-24T10:53:14.454Z  

## 文件开头预览

```ps1
$jsonData = ConvertFrom-Json ([System.IO.File]::ReadAllText('reasoning-output-Z1-Q4.json', [System.Text.Encoding]::UTF8))
$line24 = $jsonData.llmOutput
$line23 = $jsonData.thinkingChain

$cnStr = ([string][char]0x4E00) + ([string][char]0x4E8C) + ([string][char]0x4E09) + ([string][char]0x56DB) + ([string][char]0x4E94) + ([string][char]0x516D) + ([string][char]0x4E03) + ([string][char]0x516B) + ([string][char]0x4E5D) + ([string][char]0x5341)
$lu = [string][char]0x8DEF
$jing = [string][char]0x5F84
$pathPat = '#\s*' + $lu + $jing + '[' + $cnStr + ']'
$pathRe = [regex]($pathPat)

$LB = [char]0x3010
$RB = [char]0x3011

function Get-Arab([string]$cn) {
    if ($cn.Length -ne 1) { return '?' }
    $ord = [int][char]$cn
    switch ($ord) {
        19968 { return '1' }
        20108 { return '2' }
        19977 { return '3' }
        22235 { return '4' }
        20116 { return '5' }
        20845 { return '6' }
        19971 { return '7' }
        20872 { return '8' }
        20197 { return '9' }
        default { return '?' }
    }
}

function Extract-Path-Info([string]$text) {
    $matches = $pathRe.Matches($text)
    $arr = New-Object 'System.Collections.Generic.List[object]'
    for ($i = 0; $i -lt $matches.Count; $i++) {
        $start = $matches[$i].Index
        $end = if ($i+1 -lt $matches.Count) { $matches[$i+1].Index } else { $text.Length }
        $block = $text.Substring($start, $end - $start)
        $newlineIdx = $block.IndexOf("`n")
        if ($newlineIdx -gt 0) { $title = $block.Substring(0, $newlineIdx) }
        else { $title = $block.Substring(0, [Math]::Min(150, $block.Length)) }

        $cn = $matches[$i].Value.Substring($matches[$i].Value.Length - 1, 1)

        $chunkRe = [regex]($LB + $LB + '(\d+)' + $RB + $RB)
        $chunks = @()
        foreach ($cm in $chunkRe.Matches($block)) { $chunks += $cm.Groups[1].Value }
        $uniqueChunks = ($chunks | Sort-Object -Unique)

        $obj = New-Object PSObject -Property @{
            arab = Get-Arab $cn
```
