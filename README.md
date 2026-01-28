# VS Code C++ 开发环境配置指南
本文是 VS Code 配置 C++ 开发环境的踩坑记录与解决方案，包含编译、调试配置及常见问题处理。

## 一、核心配置文件
- `launch.json`：调试配置文件，需确保 `miDebuggerPath` 指向本地 `gdb.exe`。
- `tasks.json`：编译配置文件，需包含 `-g` 参数以生成调试信息。

## 二、基础操作
1. 编译：`Ctrl+Shift+B` 触发编译。
2. 调试：`F5` 启动调试，需关闭外部黑框（`externalConsole: false`）。

## 三、MinGW64 环境配置
### 1. 下载地址
官方源（较慢）：https://sourceforge.net/projects/mingw-w64/files/
国内镜像（推荐）：https://github.com/niXman/mingw-builds-binaries/releases
### 2. 安装/配置步骤
1. 下载 MinGW64 压缩包（选择 x86_64-posix-seh 版本）；
2. 解压到本地（如 `D:\mingw64`）；
3. 将 `D:\mingw64\bin` 添加到系统环境变量 PATH；
4. 验证：终端输入 `g++ --version`，显示版本号即配置成功。
