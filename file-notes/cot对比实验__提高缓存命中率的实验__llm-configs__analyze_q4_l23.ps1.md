# analyze_q4_l23.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\analyze_q4_l23.ps1`  
> **分类**: 脚本  
> **大小**: 1.9 KB  
> **最后修改**: 2026-09-24T10:53:39.271Z  

## 文件开头预览

```ps1
$jsonData = ConvertFrom-Json ([System.IO.File]::ReadAllText('reasoning-output-Z1-Q4.json', [System.Text.Encoding]::UTF8))
$line23 = $jsonData.thinkingChain
$line24 = $jsonData.llmOutput

$sb = New-Object System.Text.StringBuilder
$sep = [string]::new([char]0x3D, 100)

$null = $sb.AppendLine($sep)
$null = $sb.AppendLine('L23 STRUCTURE ANALYSIS for Z1-Q4')
$null = $sb.AppendLine($sep)
$null = $sb.AppendLine('Total length: ' + $line23.Length)
$null = $sb.AppendLine('')
$null = $sb.AppendLine('=== FIRST 500 chars ===')
$null = $sb.AppendLine($line23.Substring(0, [Math]::Min(500, $line23.Length)))
$null = $sb.AppendLine('')
$null = $sb.AppendLine('=== CHUNK 4000-4500 ===')
$null = $sb.AppendLine($line23.Substring(4000, 500))
$null = $sb.AppendLine('')
$null = $sb.AppendLine('=== CHUNK 5000-5500 ===')
$null = $sb.AppendLine($line23.Substring(5000, 500))
$null = $sb.AppendLine('')

# Find positions of key markers
$null = $sb.AppendLine('=== KEY MARKERS in L23 ===')
$LB = [char]0x3010
$RB = [char]0x3011

# Count L23 chunks
$chunkRe = [regex]($LB + $LB + '(\d+)' + $RB + $RB)
$chunks = @()
foreach ($cm in $chunkRe.Matches($line23)) { $chunks += $cm.Groups[1].Value }
$null = $sb.AppendLine('L23 chunk citations: ' + ($chunks.Count) + ' total, unique: ' + (($chunks | Sort-Object -Unique).Count))
$null = $sb.AppendLine('Unique chunks in L23: [' + (($chunks | Sort-Object -Unique) -join ', ') + ']')

$null = $sb.AppendLine('')
$null = $sb.AppendLine('=== L24 chunks ===')
$chunks24 = @()
foreach ($cm in $chunkRe.Matches($line24)) { $chunks24 += $cm.Groups[1].Value }
$null = $sb.AppendLine('L24 chunk citations: ' + ($chunks24.Count) + ' total, unique: ' + (($chunks24 | Sort-Object -Unique).Count))
$null = $sb.AppendLine('Unique chunks in L24: [' + (($chunks24 | Sort-Object -Unique) -join ', ') + ']')

[System.IO.File]::WriteAllText('q4_l23_structure.txt', $sb.ToString(), [System.Text.Encoding]::UTF8)

```
