# final_clean.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\final_clean.ps1`  
> **分类**: 脚本  
> **大小**: 6.8 KB  
> **最后修改**: 2026-09-24T10:31:45.630Z  

## 文件开头预览

```ps1
$jsonData = ConvertFrom-Json ([System.IO.File]::ReadAllText('reasoning-output-Z1-Q3.json', [System.Text.Encoding]::UTF8))
$line24 = $jsonData.llmOutput
$line23 = $jsonData.thinkingChain

$LB = [char]0x3010
$RB = [char]0x3011

$sb = New-Object System.Text.StringBuilder
$sep = [string]::new([char]0x3D, 80)
$dash = [string]::new([char]0x2D, 80)

# Build pattern with explicit chars
$cnStr = ([string][char]0x4E00) + ([string][char]0x4E8C) + ([string][char]0x4E09) + ([string][char]0x56DB) + ([string][char]0x4E94) + ([string][char]0x516D) + ([string][char]0x4E03) + ([string][char]0x516B) + ([string][char]0x4E5D) + ([string][char]0x5341)
$lu = [string][char]0x8DEF
$jing = [string][char]0x5F84
$pathPat = '#\s*' + $lu + $jing + '[' + $cnStr + ']'
$pathRe = [regex]($pathPat)

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

# Parse paths with .NET array
function ParsePaths([string]$text) {
    $matches = $pathRe.Matches($text)
    $arr = New-Object 'System.Collections.Generic.List[object]'
    foreach ($m in $matches) {
        $cn = $m.Value.Substring($m.Value.Length - 1, 1)
        $obj = New-Object PSObject -Property @{ n = $cn; p = $m.Index }
        $arr.Add($obj)
    }
    return $arr
}

$paths24 = ParsePaths $line24
$paths23 = ParsePaths $line23

```
