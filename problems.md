# asf

## 分区

## 安装输入法

主要是安装fictx5,然后配置一下文件

## 安装WPS

提到manjaro linux 缺少一个基础软件，安装后成功解决了问题。于是参照执行，果然成功了。记录一下

一，先安装这个：sudo pacman -S base-devel

二，再安装就成功了。yay -S wps-office-cn wps-office-mui-zh-cn
三，字体安装：sudo pacman -S ttf-wps-fonts

## 换源

配置源
配置中国的 mirrors，在 终端 执行下面的命令从官方的源列表中对中国源进行测速和设置：

sudo pacman-mirrors -g  # 排列源，可不执行
sudo pacman-mirrors -i -c China -m rank # 更改源，在跳出的对话框里选择想要的源
为 Manjaro 增加中文社区的源来加速安装软件，在 /etc/pacman.conf 中添加 archlinuxcn 源，末尾加上：

只能添加一个，建议官方源

[archlinuxcn]
# The Chinese Arch Linux communities packages.
# SigLevel = Optional TrustedOnly
SigLevel = Optional TrustAll
# 官方源
Server   = http://repo.archlinuxcn.org/$arch
# 163源
Server = http://mirrors.163.com/archlinux-cn/$arch
# 清华大学
Server = https://mirrors.tuna.tsinghua.edu.cn/archlinuxcn/$arch

## 安装edge等

## flameshot

sudo pacman -S flameshot

笔者这里配置的是Ctrl+Alt+A，再点击动作，配置命令/URL为/usr/bin/flameshot gui，最后应用该配置即可