# analyze.ps1

> **路径**: `analyze.ps1`  
> **分类**: 脚本  
> **大小**: 1.4 KB  
> **最后修改**: 2026-09-24T03:14:45.816Z  

## 文件开头预览

```ps1
$root = $args[0]
$bracket = [string][char]0x3010
$open = $bracket + $bracket
$dirs = Get-ChildItem -LiteralPath $root -Directory
foreach ($d in $dirs) {
    Write-Host ('=== ' + $d.Name + ' ===')
    $files = Get-ChildItem -LiteralPath $d.FullName -Filter 'call-*-response.json' | Sort-Object Name
    foreach ($f in $files) {
        $j = Get-Content -LiteralPath $f.FullName -Raw | ConvertFrom-Json
        $t = $j.response.text
        $firstThree = if ($t.Length -ge 3) { $t.Substring(0,3) } else { $t }
        $type = '?'
        if ($t -eq 'NONE') { $type = 'NONE' }
        elseif ($firstThree -eq $open) { $type = 'Recall' }
        else { $type = 'Other' }
        $reqFile = $f.FullName -replace 'response\.json$','request.json'
        $reqType = '?'
        if (Test-Path -LiteralPath $reqFile) {
            $rj = Get-Content -LiteralPath $reqFile -Raw | ConvertFrom-Json
            $pp = $rj.promptPreview
            if ($pp -match '请按重要程度打分') { $reqType = 'Score' }
            elseif ($pp -match '选出所有对回答这个问题') { $reqType = 'Recall' }
            else { $reqType = 'Unknown' }
        }
        $attempts = $j.attempts
        $retries = $j.retries
        $elapsed = $j.elapsed
        Write-Host ($j.callId + ' | resp=' + $type.PadRight(7) + ' | req=' + $reqType.PadRight(7) + ' | attempts=' + $attempts + ' retries=' + $retries + ' elapsed=' + $elapsed + 'ms')
    }
}

```
