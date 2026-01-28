# VS Code C++ 开发环境配置指南
本文是 VS Code 配置 C++ 开发环境的踩坑记录与解决方案，包含编译、调试配置及常见问题处理。

## 一、核心配置文件
- `launch.json`：调试配置文件，需确保 `miDebuggerPath` 指向本地 `gdb.exe`。
- `tasks.json`：编译配置文件，需包含 `-g` 参数以生成调试信息。

## 二、基础操作
1. 编译：`Ctrl+Shift+B` 触发编译。
2. 调试：`F5` 启动调试，需关闭外部黑框（`externalConsole: false`）。

## 三、下载资源
点击下载完整配置文档：
[VSCode-C++-Setup-Guide.docx](https://github.com/microdzh/VSCode-C--Setup/raw/main/VSCode-C++-Setup-Guide.docx)
