# test_py.cmd

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\test_py.cmd`  
> **分类**: 其他  
> **大小**: 0.2 KB  
> **最后修改**: 2026-09-24T10:18:36.173Z  

## 文件开头预览

```cmd
@echo off
set PYTHONEXE=C:\Users\Administrator\AppData\Local\Microsoft\WindowsApps\python.exe
"%PYTHONEXE%" -c "print('HELLO FROM PYTHON'); import sys; sys.stdout.flush()"
echo Done. ERRORLEVEL=%ERRORLEVEL%

```
