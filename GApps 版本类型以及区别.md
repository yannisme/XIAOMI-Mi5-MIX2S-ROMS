---
title: GApps 版本类型以及区别
tags:
  - 原创
  - GApps
url: 524.html
id: 524
categories:
  - 资源教程
abbrlink: 39907
date: 2018-07-16 22:08:51
---
# 1.Super  package
这个版本是为那些想要所有谷歌应用程序的人准备的。 它包括所有Google App 应用

- Android Messages (not installed on tablet devices) (replaces stock/AOSP SMS App)
- Android Pay
- Chrome Browser (replaces stock/AOSP Browser)
- Cloud Print
- Device Health Services
- Gmail (replaces stock/AOSP Email)
- Google+
- Google Apps Device Policy
- Google Calculator (replaces stock/AOSP Calculator)
- Google Calendar (replaces stock/AOSP Calendar)
- Google Camera (replaces stock/AOSP Camera)
- Google Connectivity Services
- Google Contacts (replaces stock/AOSP Contacts)
- Google Desk Clock (replaces stock/AOSP Desk Clock)
- Google Dialer (replaces stock/AOSP Dialer)
- Google Docs
- Google Drive
- Google Duo
- Google Earth
- Google Fitness
- Google Indic Keyboard
- Google Japanese Input
- Google Keep
- Google Keyboard (replaces stock/AOSP Keyboard)
- Google Korean Input
- Google News & Weather
- Google NFC Tags (replaces stock/AOSP NFC Tags)
- Google Now Launcher (replaces stock/AOSP Launcher)
- Google Package Installer (replaces stock/AOSP Package Installer)
- Google Pinyin Input
- Google Play Books
- Google Play Games
- Google Play Movies & TV
- Google Play Music
- Google Play Newsstand
- Google Play services
- Google Print Service Recommendation Service (replaces stock/AOSP Print Service Recommendation Service)
- Google Search
- Google Sheets
- Google Slides
- Google Storage Manager (replaces stock/AOSP Storage Manager)
- Google Street View
- Google Text-to-Speech (replaces stock/AOSP Pico TTS)
- Google VR Services
- Google Translate
- Google WebView (replaces stock/AOSP WebView)
- Google Zhuyin Input
- Hangouts
- Maps
- Pixel Icons
- Pixel Launcher (replaces stock/AOSP Launcher)
- Photos (replaces stock/AOSP Gallery)
- Project Fi by Google
- TalkBack
- Wallpapers
- YouTube

# 2.aroma package
aroma package 是一个特殊版本的常规“超级 Super”包,因为他有图形化选择前端,允许选择特定的应用程序安装，不必手工编写gapps-config文件。它是Open GApps 具备图形化安装界面，在刷入过程中可自行选择需要安装的 GApps 组件，十分好用。（经过个人测试，只适用于在可以触摸操作的recovery下刷入。）
[点击查看截屏全安装图片过程](http://imgur.com/a/gBfR6)

# 3.stock package完整包
完整包里面包含了Nexus手机里所有的谷歌服务,也就是谷歌的核心服务，主要都有以下Google Play应用：

- Android Messages (not installed on tablet devices) (replaces stock/AOSP SMS App)
- Chrome Browser (replaces stock/AOSP Browser)
- Cloud Print
- Device Health Services
- Gmail (replaces stock/AOSP Email)
- Google+
- Google Calculator (replaces stock/AOSP Calculator)
- Google Calendar (replaces stock/AOSP Calendar)
- Google Camera (replaces stock/AOSP Camera)
- Google Contacts (replaces stock/AOSP Contacts)
- Google Desk Clock (replaces stock/AOSP Desk Clock)
- Google Dialer (replaces stock/AOSP Dialer)
- Google Docs
- Google Drive
- Google Duo
- Google Fitness
- Google Keep
- Google Keyboard (replaces stock/AOSP Keyboard)
- Google News & Weather
- Google NFC Tags (replaces stock/AOSP NFC Tags)
- Google Now Launcher (replaces stock/AOSP Launcher)
- Google Package Installer (replaces stock/AOSP Package Installer)
- Google Play Books
- Google Play Games
- Google Play Movies & TV
- Google Play Music
- Google Play Newsstand
- Google Play services
- Google Print Service Recommendation Service (replaces stock/AOSP Print Service Recommendation Service)
- Google Search
- Google Sheets
- Google Slides
- Google Storage Manager (replaces stock/AOSP Storage Manager)
- Google Text-to-Speech (replaces stock/AOSP Pico TTS)
- Google VR Services
- Google WebView (replaces stock/AOSP WebView)
- Hangouts
- Maps
- Messenger (not installed on tablet devices) (replaces stock/AOSP SMS App)
- Pixel Icons
- Pixel Launcher (replaces stock/AOSP Launcher)
- Photos (replaces stock/AOSP Gallery)
- TalkBack
- Wallpapers
- YouTube

# 4.full modular package全模块包
与 stock 完整版所包含的内容相同，但是不包含：Google 相机, Google 输入法, Google Gallery², 并且不会替换掉自带的启动器，输入法，浏览器，短信应用，或者Pico TTS服务。此外全模块包还包含Google Bookmarks 同步服务。如果你想体验Nexus手机的谷歌服务，并且想继续使用原手机自带的启动器等服务，全模块包是最好的选择。

- Android Messages (not installed on tablet devices)
- Chrome Browser
- Cloud Print
- Device Health Services
- Gmail
- Google+
- Google Calculator (replaces stock/AOSP Calculator)
- Google Calendar (replaces stock/AOSP Calendar)
- Google Desk Clock (replaces stock/AOSP Desk Clock)
- Google Docs
- Google Drive
- Google Fitness
- Google Keep
- Google News & Weather
- Google NFC Tags (replaces stock/AOSP NFC Tags)
- Google Now Launcher
- Google Play Books
- Google Play Games
- Google Play Movies & TV
- Google Play Music
- Google Play Newsstand
- Google Play services
- Google Search
- Google Sheets
- Google Slides
- Google Text-to-Speech
- Maps
- Photos
- TalkBack
- YouTube

# 5.mini package轻量包
包含了完整的 Google 服务框架和主流 Google 应用，去掉了 Google Docs 等文档处理应用，适合不太经常使用谷歌应用的人。轻量模块包包含有：谷歌核心服务, Google Bookmarks 同步服务, 以及以下的Google Play应用：

- Android Messages (not installed on tablet devices)
- Device Health Services
- Google Calculator (replaces stock/AOSP Calculator)
- Google Calendar (replaces stock/AOSP Calendar)
- Google Desk Clock (replaces stock/AOSP Clock)
- Google NFC Tags (replaces stock/AOSP NFC Tags)
- Google Now Launcher
- Google Package Installer (replaces stock/AOSP Package Installer)
- Google Play services
- Google Search
- Google Text-to-Speech
- Gmail
- Maps
- Photos
- YouTube

# 6.micro package迷你模块包
这个包是专为喜欢简约的用户准备的。它包含有：谷歌核心服务, Google Bookmarks 同步服务, 以及以下的Google Play应用：

- Device Health Services
- Google Calendar (replaces stock/AOSP Calendar)
- Google Now Launcher
- Google Package Installer
- Google Play services
- Google Search
- Google Text-to-Speech
- Gmail

# 7.nano package超小模块包
虽说是超小，但也包含了完整的 Google 服务框架，并不包含多余的 Google 应用。
这个包适合那些不想占用太大内存，但是又想体验到原生的谷歌搜索服务的机友。超小模块包包含有：谷歌核心服务, 

- Device Health Services
- Google Package Installer (replaces stock/AOSP Package Installer)
- Google Play services
- Google Search

# 8.pico modular package核心模块包
包含了最基础的 Google 服务框架，体积最小，适合仅仅想给系统装个Play商店的同学，其他的Google play应用可以自己下载。核心包包含有：

- Google Package Installer (replaces stock/AOSP Package Installer)
- Google Play services

# 9.TVStock Package
这个包是为Android电视设备。 它包括Nexus的所有应用。

- Android TV Customization
- Android TV Widget
- Gamepad Pairing Service
- Global Key Interceptor
- Landscape Wallpaper
- Leanback Keyboard
- Overscan Calibrator
- Pairing Tutorial
- Remote Control Service
- Second Screen Setup
- Second Screen Setup Auth Bridge
- TV Voice Input  

and the following Play Store applications:  

- Android TV Launcher
- Android TV Remote Control
- Backdrop Daydream
- Google Cast Receiver
- Google Play Games
- Google Play Movies & TV
- Google Play Music
- Google Search
- Google Webview
- Live Channels
- TalkBack
- TV Recommendations
- YouTube