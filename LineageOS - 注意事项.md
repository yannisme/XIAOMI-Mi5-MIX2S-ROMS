---
title: LineageOS 注意事项
categories:
  - 资源教程
toc: true
abbrlink: 59968
date: 2017-08-17 16:14:46
urlname:
tags:
  - ROM
  - 小米5
  - 原创
  - 汇总
---

### 可能遇到的问题请仔细阅读以下“说明”
- 错误7 需要刷入[固件-Firmware](../62258/)
- substratum主题管理器应用会导致重启后无法进入系统，现版本请勿使用
- 设置向导停止运行解决方法：不连wifi，拔出sim卡，一路通过完成向导再插卡 - staydayll
- 双卡其一为电信卡放卡1槽，并将首选网络制式改为“全球”
- **流量关闭后仍有流量偷跑无法关闭，请检查以下设置是否有关闭“增强型 4G LTE 模式”**
- 通知栏信号叉叉请使用“CaptiveMgr-清除叹号”
- 第一次刷机截图和相册功能需重启
- 支持OTA；不支持OMS和联系人直接使用sim卡导入
>要先进入系统后 (引导界面) 才能刷GApps，不然WIFI/流量处会直接跳到
谷歌验证导致无法连接谷歌服务器从而无法进入系统

****
[dwarning title=以上内容为旧版本的注意说明 font=red bg=white border=white]此提示以下为新的说明，更新于2018-01-29 ** | **电信卡设置说明请前往“传送门”中查看
**ROM OS Version: 7.x Nougat**
**ROM Kernel: Linux 3.18.x**[/dwarning]

**兼容性问题：**

- 支持所有小米5设备( 32GB / 64GB / 128GB ) . 小米 5S 和 5S Plus 不支持 
- Compatible with all Xiaomi Mi 5 variants ( 32GB / 64GB / 128GB ) . Xiaomi Mi 5S and 5S Plus are not supported.
- [英文说明](https://wiki.lineageos.org/devices/gemini/install)

**刷机过程：**

- 重启到REC（确保该Rec支持刷入7.x），然后三清 /system, /data 和 /cache，安装 Lineageos15 安装包
- 若刷入出现错误7，请刷入固件 MIUI 8.1.4 dev 包后紧接着刷入此ROM即可
Builds are based off the Xiaomi's Android 7.0 firmware with proprietary blobs from MIUI 8.1.4 dev package.

**可用方面：**

- Camera (and flashlight)，WiFi，NFC，Bluetooth，Telephony (Calls and Data)，Audio (Record and Playback)，Video Playback，Sensors，GPS，VoLTE 等等，除了不可用的东西之外都正常工作

**BUG和不可用方面：**

- 暂无

---
lineage-14.1-20180110 版本之后需要刷入 **固件 MIUI 8.1.4 dev** 之后才能刷入LOS，前往固件分类中下载相关dev固件

---
>点击 [传送门](../44321/) 获取ROM 😶 /  [更新日志](https://download.lineageos.org/gemini/changes/) 