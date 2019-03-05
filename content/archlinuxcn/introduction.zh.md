---
title: "ArchLinux CN镜像使用指南"
type : "post"
---
## 地址
http://mirrors.cqu.edu.cn/archlinuxcn/
## 说明
Arch Linux CN仓库
## 简介
Arch Linux 中文社区仓库是由 Arch Linux 中文社区驱动的非官方用户仓库。包含中文用户常用软件、工具、字体/美化包等。

仓库地址：[http://repo.archlinuxcn.org](http://repo.archlinuxcn.org)
## 收录框架
x86_64
## 使用说明
以root身份手动编辑文件 **/etc/pacman.conf**，在文件末尾加入
```bash
[archlinuxcn]
SigLevel = TrustedOnly
Server = https://mirrors.ustc.edu.cn/archlinuxcn/$arch
```
执行：
```bash
pacman -Syy
```
强制刷新软件源。
再执行：
```bash
pacman -S archlinuxcn-keyring
```
添加archlinuxCN的GPG key
<div class="alert rounded-0 alert-info">
SigLevel建议为TrustedOnly
</div>
## 相关链接
Arch Linux 中文社区主页:</br>
[https://www.archlinuxcn.org](https://www.archlinuxcn.org)</br>
Arch Linux 中文社区仓库 / 镜像加速源介绍:</br>
[https://www.archlinuxcn.org/archlinux-cn-repo-and-mirror/](https://www.archlinuxcn.org/archlinux-cn-repo-and-mirror/)
