# trace_mapper.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\trace_mapper.ps1`  
> **分类**: 脚本  
> **大小**: 11.7 KB  
> **最后修改**: 2026-09-24T12:15:52.398Z  

## 文件开头预览

```ps1
param([string]$InputFile, [string]$OutputDir = "")

$ErrorActionPreference = 'Stop'

# Load JSON
$raw = [System.IO.File]::ReadAllText($InputFile, [System.Text.Encoding]::UTF8)
$data = $raw | ConvertFrom-Json
$l23 = [string]$data.thinkingChain
$l24 = [string]$data.llmOutput
$l23Len = $l23.Length
$l24Len = $l24.Length

# Char codes (use only ASCII literals for code, char() for data)
$LB  = [char]0x3010   # left bracket
$RB  = [char]0x3011   # right bracket
$NL  = [char]10       # newline
$LU  = [char]0x8DEF   # lu char
$JING = [char]0x5F84  # jing char
$CN_NUMS = ([char]0x4E00) + ([char]0x4E8C) + ([char]0x4E09) + ([char]0x56DB) + ([char]0x4E94) + ([char]0x516D) + ([char]0x4E03) + ([char]0x516B) + ([char]0x4E5D) + ([char]0x5341)
$LBB = $LB + $LB
$RBB = $RB + $RB
$LBC = $LB            # for markdown output
$RBC = $RB            # for markdown output

# Step 1: find all single-bracket mentions in L23
$l23Mentions = @{}
$pos = 0
while ($pos -lt $l23Len) {
    $lbIdx = $l23.IndexOf($LB, $pos)
    if ($lbIdx -lt 0) { break }
    $endIdx = $l23.IndexOf($RB, $lbIdx + 1)
    if ($endIdx -lt 0) { break }
    $inner = $l23.Substring($lbIdx + 1, $endIdx - $lbIdx - 1)
    if ($inner -match '^\d+$') {
        if (-not $l23Mentions.ContainsKey($inner)) {
            $l23Mentions[$inner] = New-Object System.Collections.Generic.List[int]
        }
        $l23Mentions[$inner].Add($lbIdx)
    }
    $pos = $lbIdx + 1
}

# Step 2: find L24 paths and double-bracket chunks
$paths = New-Object System.Collections.Generic.List[Hashtable]

# Build line starts
$lineStarts = New-Object System.Collections.Generic.List[int]
$lineStarts.Add(0)
for ($i = 0; $i -lt $l24Len; $i++) {
    if ($l24[$i] -eq $NL) { $lineStarts.Add($i + 1) }
```
