# find_py.cmd

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\find_py.cmd`  
> **分类**: 其他  
> **大小**: 0.2 KB  
> **最后修改**: 2026-09-24T10:19:04.603Z  

## 文件开头预览

```cmd
@echo off
where python
echo --------
where python.exe
echo --------
where python3
echo --------
dir "C:\Python*" 2>nul
echo --------
dir "C:\Users\Administrator\AppData\Local\Microsoft\WindowsApps\python*" 2>nul
echo --------
echo PATH:
echo %PATH%

```
