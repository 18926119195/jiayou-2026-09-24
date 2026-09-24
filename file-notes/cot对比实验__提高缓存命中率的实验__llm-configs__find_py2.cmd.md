# find_py2.cmd

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\find_py2.cmd`  
> **分类**: 其他  
> **大小**: 0.2 KB  
> **最后修改**: 2026-09-24T10:19:40.629Z  

## 文件开头预览

```cmd
@echo off
dir C:\Python* 2>nul
dir "C:\Program Files\Python*" 2>nul
dir "C:\Users\Administrator\AppData\Local\Programs\Python*" 2>nul
dir "C:\ProgramData\Anaconda*" 2>nul
dir "C:\Anaconda*" 2>nul
where pip 2>nul
where py 2>nul

```
