# run_debug.cmd

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\run_debug.cmd`  
> **分类**: 其他  
> **大小**: 0.3 KB  
> **最后修改**: 2026-09-24T10:15:07.645Z  

## 文件开头预览

```cmd
@echo off
set PY=C:\Users\Administrator\AppData\Local\Microsoft\WindowsApps\python.exe
cd /d "C:\Users\Administrator\Desktop\chenggong-jiachi-master\cot对比实验\提高缓存命中率的实验\llm-configs"
"%PY%" debug_l24.py
echo Exit code: %ERRORLEVEL%

```
