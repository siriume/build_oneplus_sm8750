**`简体中文`** | [English](README-en.md)<br>

[![GitHub](https://img.shields.io/badge/-GitHub|@siriume-181717?logo=github&logoColor=white&style=flat-square)](https://github.com/siriume/build_oneplus_sm8750)
[![一加内核开源地址](https://img.shields.io/badge/一加内核开源地址-EB0029?logo=oneplus&logoColor=white&style=flat-square)](https://github.com/OnePlusOSS/kernel_manifest)
<br><b>本项目构建支持来自</b>[![GitHub](https://img.shields.io/badge/-GitHub|@HanKuCha-181717?logo=github&logoColor=white&style=flat-square)](https://github.com/HanKuCha/oneplus13_a5p_sukisu)<br>
# 本地脚本使用方法
> ⚠️ 注意：如果想使用自己fork的仓库进行编译，fork时如更改了仓库名，请将下方“使用方法”中的 `build_oneplus_sm8750` 改成你修改后的项目名并将下方链接中的 `siriume` 改成你的 GitHub 用户名。  
> 比如你的用户名是 `abcd`，仓库名为`123456`则命令为：  
> `git clone https://github.com/abcd/123456.git`
---
```bash
git clone https://github.com/siriume/build_oneplus_sm8750.git
```
```bash
cd build_oneplus_sm8750
```
```bash
chmod +x Build_sm8750.sh
```
```bash
./Build_sm8750.sh
```

---

## Windows推荐使用WSL运行  
这里提供WSL迁移到其他盘（如E盘）的方法，避免占用C盘空间。

### WSL2迁移至其他目录步骤

1. 以管理员身份打开 PowerShell，查看当前WSL版本：

```powershell
wsl -l -v
```

2. 停止所有正在运行的WSL实例：

```powershell
wsl --shutdown
```

3. 导出你想迁移的Linux发行版（例如Ubuntu-20.04）：

```powershell
wsl --export Ubuntu-20.04 E:/ubuntu.tar
```

4. 注销原有Linux发行版：

```powershell
wsl --unregister Ubuntu-20.04
```

5. 将导出的发行版导入到新的目录：

```powershell
wsl --import Ubuntu-20.04 E:\ubuntu\ E:\ubuntu.tar --version 2
```

6. 设置默认用户：

```powershell
ubuntu2004.exe config --default-user <username>
```

>请将 `<username>` 替换为你WSL安装时设置的用户名。  
>例如我的用户名是 `qiudaoyu`，则命令为：
```powershell
ubuntu2004.exe config --default-user qiudaoyu
```

---

