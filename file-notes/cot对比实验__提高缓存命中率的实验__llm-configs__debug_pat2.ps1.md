# debug_pat2.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\debug_pat2.ps1`  
> **分类**: 脚本  
> **大小**: 2.5 KB  
> **最后修改**: 2026-09-24T10:27:22.366Z  

## 文件开头预览

```ps1
$content = [System.IO.File]::ReadAllText('reasoning-output-Z1-Q3.json', [System.Text.Encoding]::UTF8)
$lines = $content -split "`n"
$line24 = $lines[23]
$line23 = $lines[22]

$LB = [char]0x3010
$RB = [char]0x3011

$sb = New-Object System.Text.StringBuilder
$sep = [string]::new([char]0x3D, 78)
$dash = [string]::new([char]0x2D, 78)
$null = $sb.AppendLine($sep)
$null = $sb.AppendLine('L24 -> L23 PATH MAPPING')
$null = $sb.AppendLine($sep)

# Use simpler approach - match with char codes from string
# 路 = U+8DEF, 径 = U+5F84, 一-十 covers specific code points
# Use [0-9] just to test if regex works at all
$r1 = [regex]('#\s*[\u8def]\u8def\u5f84')  # Just testing if \u escapes work
$null = $sb.AppendLine('Test1 (\\u8def\\u5f84): ' + $r1.Matches($line24).Count + ' matches')

# Now use char class with explicit Chinese nums
# Build the pattern by adding chars one at a time
$lu = [string][char]0x8DEF
$jing = [string][char]0x5F84
$cnNums = @()
$cnNums += [string][char]0x4E00  # 1
$cnNums += [string][char]0x4E8C  # 2
$cnNums += [string][char]0x4E09  # 3
$cnNums += [string][char]0x56DB  # 4
$cnNums += [string][char]0x4E94  # 5
$cnNums += [string][char]0x516D  # 6
$cnNums += [string][char]0x4E03  # 7
$cnNums += [string][char]0x516B  # 8
$cnNums += [string][char]0x4E5D  # 9
$cnNums += [string][char]0x5341  # 10
$cnStr = [string]::Join('', $cnNums)
$null = $sb.AppendLine('cnStr: ' + $cnStr + ' (length=' + $cnStr.Length + ')')

# Build pattern with explicit char codes
$pat = '#\s*' + $lu + $jing + '[' + $cnStr + ']'
$null = $sb.AppendLine('pattern: ' + $pat)
$r2 = [regex]($pat)
$null = $sb.AppendLine('Test2 pattern matches: ' + $r2.Matches($line24).Count)

# Try escape syntax explicitly
$patEsc = '#\s*' + $lu + $jing + '[\u4e00\u4e8c\u4e09\u56db\u4e94\u516d\u4e03\u516b\u4e5d\u5341]'
$r3 = [regex]($patEsc)
$null = $sb.AppendLine('Test3 (escape) matches: ' + $r3.Matches($line24).Count)

```
