# find_tools.cmd

> **路径**: `cot对比实验\提高缓存命中率的实验\llm-configs\find_tools.cmd`  
> **分类**: 其他  
> **大小**: 0.2 KB  
> **最后修改**: 2026-09-24T10:20:11.239Z  

## 文件开头预览

```cmd
@echo off
where uv 2>nul
where uvx 2>nul
where py 2>nul
where pip 2>nul
where pip3 2>nul
where conda 2>nul
where node 2>nul
dir "%USERPROFILE%\.local\bin" 2>nul
echo --
echo done

```
