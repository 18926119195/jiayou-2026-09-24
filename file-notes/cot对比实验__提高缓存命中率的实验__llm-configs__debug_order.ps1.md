# debug_order.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\debug_order.ps1`  
> **分类**: 脚本  
> **大小**: 1.5 KB  
> **最后修改**: 2026-09-24T10:30:28.012Z  

## 文件开头预览

```ps1
$jsonData = ConvertFrom-Json ([System.IO.File]::ReadAllText('reasoning-output-Z1-Q3.json', [System.Text.Encoding]::UTF8))
$line24 = $jsonData.llmOutput
$line23 = $jsonData.thinkingChain

$LB = [char]0x3010
$RB = [char]0x3011

$sb = New-Object System.Text.StringBuilder

$lu = [string][char]0x8DEF
$jing = [string][char]0x5F84
$cnStr = ([string][char]0x4E00) + ([string][char]0x4E8C) + ([string][char]0x4E09) + ([string][char]0x4E00) + ([string][char]0x56DB) + ([string][char]0x4E94) + ([string][char]0x516D) + ([string][char]0x4E03) + ([string][char]0x516B) + ([string][char]0x4E5D) + ([string][char]0x5341)

# Hmm wait, I duplicated 0x4E00. Let me redo
$cnStr = ([string][char]0x4E00) + ([string][char]0x4E8C) + ([string][char]0x4E09) + ([string][char]0x56DB) + ([string][char]0x4E94) + ([string][char]0x516D) + ([string][char]0x4E03) + ([string][char]0x516B) + ([string][char]0x4E5D) + ([string][char]0x5341)
$null = $sb.AppendLine('cnStr: "' + $cnStr + '" length=' + $cnStr.Length)

$pathPat = '#\s*' + $lu + $jing + '[' + $cnStr + ']'
$pathRe = [regex]($pathPat)

$ms = $pathRe.Matches($line24)
$null = $sb.AppendLine('L24 matches: ' + $ms.Count)
foreach ($m in $ms) {
    $txt = $m.Value
    $lastChar = $txt.Substring($txt.Length - 1, 1)
    $ord = [int][char]$lastChar
    $null = $sb.AppendLine('  pos ' + $m.Index + ': "' + $txt + '" lastChar="' + $lastChar + '" ord=' + $ord)
}

[System.IO.File]::WriteAllText('debug_order.txt', $sb.ToString(), [System.Text.Encoding]::UTF8)

```
