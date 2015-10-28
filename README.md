# OpenWrt-HiWiFi
OpenWrt-HiWiFi is forked from OpenWrt
It is a branch of HiWiFi-HC5661 based on OpenWrt
## About HiWiFi
* Official website: [http://www.hiwifi.com/](http://www.hiwifi.com/)

***
## Introduction
* Include HiWiFi-HC5661 dts file and profile
* Support HiWiFi bdinfo
* Support HiWiFi flash layout
* Build-in LuCi Background Interface
## Checkout code
```
# Install essential software
sudo apt-get install build-essential git subversion wget flex gettext libncurses5-dev unzip gawk liblzma-dev zlib1g-dev ccache u-boot-tools
git clone https://github.com/ChasonTang/OpenWrt-HC5661.git
```
## Pre-Compile
```
cd OpenWrt-HC5661
# feed update
./script/feed update -a
./script/feed install -a
make menuconfig
# n is your cpu number
make V=s -jn
```
