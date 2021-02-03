# mingw-w64-clang
**在 MSYS2 中安装 [Clang](https://clang.llvm.org/index.html) 的教程**

一直以来，Windows 安装 [Clang](https://clang.llvm.org/index.html) 非常难。但现在，[MSYS2](https://www.msys2.org/)可以让我们方便地安装 Clang。  

## 步骤

### 第一步：安装 MSYS2
请前往 <https://www.msys2.org/> 下载安装。

### 第二步：更换软件源（可选）
国内用户由于网络速度慢，可以尝试切换为国内的软件源。  
[**点击前往百度搜索**](https://www.baidu.com/s?ie=UTF-8&wd=MSYS2%E6%9B%B4%E6%8D%A2%E8%BD%AF%E4%BB%B6%E6%BA%90)

### 第三步：安装 Clang

#### MinGW 32-bit

1. 从“开始”菜单启动 MSYS2 MinGW 32-bit。
1. 输入以下命令后按回车：`pacman -S mingw-w64-i686-clang`
1. 键入“Y”并回车。
1. 静静等待。
1. 完成后，输入 `clang --version` 测试安装。
如果出现类似于下面的声明，证明你安装成功了！
```
$ clang --version
clang version 11.0.0 (https://github.com/msys2/MINGW-packages c0083b9edc111315c868f9c53dd60aaa78d1669b)
Target: i686-w64-windows-gnu
Thread model: posix
InstalledDir: C:\msys64\mingw32\bin
```

#### MinGW 64-bit

1. 从“开始”菜单启动 MSYS2 MinGW 64-bit。
1. 输入以下命令后按回车：`pacman -S mingw-w64-x86_64-clang`
1. 键入“Y”并回车。
1. 静静等待。
1. 完成后，输入 `clang --version` 测试安装。
如果出现类似于下面的声明，证明你安装成功了！
```
$ clang --version
clang version 11.0.0 (https://github.com/msys2/MINGW-packages c0083b9edc111315c868f9c53dd60aaa78d1669b)
Target: x86_64-w64-windows-gnu
Thread model: posix
InstalledDir: C:\msys64\mingw64\bin
```
