---
title: LineageOS 15.0 注意事项
categories:
  - 资源教程
toc: true
abbrlink: 64619
date: 2017-09-29 12:22:52
urlname:
tags:
  - ROM
  - 小米5
  - 原创
  - 汇总
---
### 可能遇到的问题请仔细阅读以下“说明”

- 目前的LineageOS 15.0 是非官方版基于安卓8.0 (奥利奥) 
- VoLTE 不可用 **[📍 10-31版本以上相机可用]**
- 需要固件版本为 `MIUI 7.7.6全球开发版` ,否则安装会失败
- 刷入20171031后声音功能不正常是BUG，按二楼方法修复

**电话问题：具体步骤就是进入移动网络设置里面，最开始那个首选网络会显示为LTE，然后你点开后关闭，就会自动变成通用，然后再`*#*#4636#*#*`里面，设置网络选项为`LTE\TD-CDMA\WCDMA`这一项就好了。- 感谢"winslowkin"**

****
[dwarning title=以上内容为旧版本的注意说明 font=red bg=white border=white]此提示以下为新的说明，更新于2018-01-27** | **电信卡设置说明请前往“传送门”中查看
**ROM 版本: 8.1 Oreo**
**ROM 内核: Linux 3.18.x**[/dwarning]

**兼容性问题：**

- 支持所有小米5设备( 32GB / 64GB / 128GB ) . 小米 5S 和 5S Plus 不支持
- Compatible with all Xiaomi Mi 5 variants ( 32GB / 64GB / 128GB ) . Xiaomi Mi 5S and 5S Plus are not supported.

**刷机过程：**

- 重启到REC，然后三清 /system, /data 和 /cache，安装 Lineageos15 安装包
- 若刷入出现错误7，请刷入固件 MIUI 8.1.4 dev 包后紧接着刷入此ROM即可
Builds are based off the Xiaomi's Android 7.0 firmware with proprietary blobs from MIUI 8.1.4 dev package.

**可用方面：**

- Camera (and flashlight)，WiFi，NFC，Bluetooth，Telephony (Calls and Data)，Audio (Record and Playback)，Video Playback，Sensors，GPS，VoLTE

**BUG和不可用方面：**

- 暂无

***
>点击 [传送门](../44321/) 获取ROM 😶 | [固件获取](https://me-1.cn/d/9-firmware)