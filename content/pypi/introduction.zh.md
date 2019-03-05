---
title: "PyPi镜像使用指南"
description: "Python的额外工具库"
type : "post"
---
临时使用
```
pip install -i https://mirrors.hexang.com/pypi/web/simple/ some-package
```
注意，simple 不能少, 是 ***https*** 而不是 http

设为默认
修改 **~/.pip/pip.conf** ，如果文件不存在则执行：
```
touch ~/.pip/pip.conf
```
修改 index-url 如下：
```
[global]
index-url = https://mirrors.hexang.com/pypi/web/simple/
```
