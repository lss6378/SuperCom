---
description: SuperCom 项目构建指南
---

## 快速开始

```bash
# 进入项目目录
cd d:\playground\UartAssert\SuperCom

# 构建调试版本
MSBuild.exe /p:Configuration=Debug /p:Platform="Any CPU"

# 运行程序
cd SuperCom\bin\Debug
SuperCom.exe
```

## 常用命令

### 调试版本
```bash
MSBuild.exe /p:Configuration=Debug /p:Platform="Any CPU"
```

### 发布版本
```bash
MSBuild.exe /p:Configuration=Release /p:Platform="Any CPU"
```

### 清理解决方案
```bash
MSBuild.exe /t:Clean /p:Configuration=Debug /p:Platform="Any CPU"
```

## 输出目录
- 调试版本: `SuperCom\bin\Debug`
- 发布版本: `SuperCom\bin\Release`

## 常见问题
- 确保已安装 .NET Framework 4.7.2+
- 缺少依赖时提示报错
- 构建异常时删除 `bin` 和 `obj` 文件夹后重试
   ```
