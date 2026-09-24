# verify-reorder.ps1

> **路径**: `cot对比实验\提高缓存命中率的实验\verify-reorder.ps1`  
> **分类**: 脚本  
> **大小**: 4.0 KB  
> **最后修改**: 2026-09-24T06:24:25.497Z  

## 文件开头预览

```ps1
# 纯字节级校验 - 完全基于原始字节，不做字符串解释
[Console]::OutputEncoding = [System.Text.Encoding]::UTF8
$OutputEncoding = [System.Text.Encoding]::UTF8
$utf8 = [System.Text.Encoding]::UTF8

$SRC = 'C:\Users\Administrator\Desktop\chenggong-jiachi-master\cot对比实验'
$OUT_DIR = 'C:\Users\Administrator\Desktop\chenggong-jiachi-master\cot对比实验\提高缓存命中率的实验'

# marker 字节序列 (UTF-8):  【【全量材料】】
#  【 = E3 80 90 (0x3010)
#  】 = E3 80 91 (0x3011)
#  全 = E5 85 A8 (0x5168)
#  量 = E9 87 8F (0x91CF)
#  材 = E6 9D 90 (0x6750)
#  料 = E6 96 99 (0x6599)
$MARKER_BYTES = [byte[]](
  0xE3,0x80,0x90,    # 【
  0xE3,0x80,0x90,    # 【
  0xE5,0x85,0xA8,    # 全
  0xE9,0x87,0x8F,    # 量
  0xE6,0x9D,0x90,    # 材
  0xE6,0x96,0x99,    # 料
  0xE3,0x80,0x91,    # 】
  0xE3,0x80,0x91     # 】
)

function Find-BytesInBytes([byte[]]$haystack, [byte[]]$needle) {
  for ($i = 0; $i -le $haystack.Length - $needle.Length; $i++) {
    $match = $true
    for ($j = 0; $j -lt $needle.Length; $j++) {
      if ($haystack[$i + $j] -ne $needle[$j]) { $match = $false; break }
    }
    if ($match) { return $i }
  }
  return -1
}

function Compare-ByteRanges([byte[]]$a, [byte[]]$b) {
  if ($a.Length -ne $b.Length) { return $false }
  for ($i = 0; $i -lt $a.Length; $i++) {
    if ($a[$i] -ne $b[$i]) { return $false }
  }
  return $true
}

function Copy-ByteRange([byte[]]$src, [int]$start, [int]$len) {
  $dst = New-Object 'byte[]' $len
  [Array]::Copy($src, $start, $dst, 0, $len)
  return $dst
}
```
