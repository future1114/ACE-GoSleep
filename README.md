# GoSleepace 进程监控工具 v1.0

---

## 【免责声明】
本工具仅供学术研究和技术探讨使用。
用户应遵守当地法律法规，不得用于非法用途。
使用本工具所产生的一切后果由使用者自行承担。

---

## 【GitHub 下载与依赖】
### 1. 工具下载
- 直接下载压缩包：[ACE_GoSleep.7z]
- 或前往 GitHub Releases 页面下载最新版本：[Releases]https://github.com/future1114/ACE-GoSleep/releases/tag/Init)

### 2. 运行依赖
本项目基于 **.NET 9.0** 开发，运行前需确保系统已安装以下运行时：
- 依赖包名称：`aspnetcore-runtime-9.0.10-win-x64.zip`
- 下载方式：
  1. 官网下载（推荐）：[.NET 9.0 运行时官网](https://dotnet.microsoft.com/zh-cn/download/dotnet/9.0)
  2. 项目提供的备用包：可直接下载 `aspnetcore-runtime-9.0.10-win-x64.zip`

---

## 【如何运行】

### 方式1（推荐，最简单）：
1. 解压下载的 `ACE_GoSleep.7z` 压缩包
2. 右键点击解压后的 `GoSleepace.exe`
3. 选择"以管理员身份运行"

### 方式2：
1. 解压 `ACE_GoSleep.7z` 压缩包
2. 双击运行解压目录中的 `Run-AsAdmin.bat`

### 方式3：
1. 解压 `ACE_GoSleep.7z` 压缩包
2. 以管理员身份打开命令提示符（CMD/PowerShell）
3. 切换到解压目录，运行命令：`GoSleepace.exe`

---

## 【启动后】
- 控制台显示免责声明和系统信息（2行2列格式）
- Web控制面板：[http://localhost:5000](http://localhost:5000)
- 按 `y` 键执行检查任务
- 按 `q` 键退出程序

---

## 【配置】
编辑解压目录下的 `appsettings.json` 文件，可自定义以下参数：
- 目标进程列表（需监控的进程名称）
- CPU核心设置（指定使用的CPU核心数）
- 能效模式开关（开启/关闭节能模式）
- 监控间隔（进程检查的时间间隔，单位：秒）
- Web服务器端口（默认5000，可修改为其他空闲端口）

---

## 【系统要求】
- 操作系统：Windows 10 1903 或更高版本（64位）
- 权限要求：必须以管理员身份运行
- 硬件要求：兼容x64架构的CPU，至少2GB内存

---

### 备注
1. 若运行时提示"缺少.NET运行时"，请先安装上述依赖包
2. 压缩包解压后建议保留完整目录结构，避免文件丢失导致程序异常
3. 如需提交Issue或贡献代码，可前往GitHub仓库：[项目仓库地址](https://github.com/future1114/ACE-GoSleep)