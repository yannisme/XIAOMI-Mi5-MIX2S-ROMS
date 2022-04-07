---
title: Pure OS 注意事项
categories:
  - 资源教程
toc: true
abbrlink: 33453
date: 2017-11-17 13:56:41
urlname:
tags:
  - ROM
  - 小米5
  - 原创
  - 汇总
---
>Disclaimer: We are not responsible if you destroy your device. Use at your own risk.
免责声明：若您的设备损坏，对此Pure OS不予负责；请自己承担风险。

- ROOT可刷入：SuperSU-v2.82
- 系统无默认短信/相机/浏览器/Google Shop, 需自行安装短信/相机/浏览器等软件，可通过蓝牙或电脑传入
- 耗电问题请配合黑域等小黑屋进行优化
- 无拼音T9搜索/无谷歌全家桶, 需要自行刷入GApps(可刷7.1版本的GApps)
- 可用相机/手电
- 可用电信卡
 - 电信卡一主卡，副卡其他除电信外，将网络类型调为通用，详细办法请查看传送门总汇贴中的链接

***
>点击 [传送门](../44321/) 获取ROM 😶 

***
## General
·Based on AOSP Android 7.1.2
·Busybox, and Init.d support
·Pixel sounds and OEM wallpapers from factory images
·Pixel theme and Pixel navbar animation
·Pixel colors
·Bug fix's and stability improvements
·UI Improvements (fixed a bunch google forgot to materialize)
·Rootless Substratum OMS Theme Engine support
·ADB enhancements (ADB over wifi, Hide ADB icon, colored logcat "abd logcat -C")
·Developer settings by default
·Enabled Night mode for all devices
·Custom night light brightness options
·Disabled forced encryption
·Disabled tether provision checks
·Download speed in notification
·Advanced reboot menu
·Advanced screenshot functionality (longpress tile/power menu for selectable screenshot)
·Back volume adjust sounds and toggle
·Advanced rotation control and lockscreen rotation toggle
·Ability to lock app in landscape via rotation tile
·Advanced charging sound controls
·Advanced seekbar style animation controls
·Quick setting header Longpress actions
·Ability to see app version when sideloading app
·App package name to app info screen
·Ability to launch app when touching app icon in app info screen
·Phone info shortcut to about phone/status on top
·Dynamic vendor image notification
·Additional battery saver trigger steps
·Ability to unlink notification volume from ringer volume
·Increasing ringtone option

## Lock Screen
·Lockscreen item option(time, date, alarm text toggles & Clock font style)
·Double tap anywhere to sleep
·Long press power for torch
·Option to disable lockscreen media art
·Option to scramble the pin entry layout
·Option to disable the pin ripple background when entering lockscren pin
·Option to disable fingerprint success vibration

## Notification Drawer
·Quick settings pulldown (left,right,always)
·Smart pulldown (no ongoing, no dismissable, no notifications)
·Advanced quick settings easy toggle
·Brightness slider on/off toggle
·Haptic feedback on quick setting on/off toggle
·Ability to disable quick settings on secure lockscreen
·Ability to disable the quick settings title text
·Ability to change number of quick settings columns
·Ability to change the amount of rows in quick settings
·Ability to set contexual or custom header images

## Recent apps
·Immersive recents
·Kill all fab
·Kill all fab location

## Statusbar
·Battery customization(percentage/icon style)
·Sync battery icon with quick settings tile
·Battery bar options(location, color, style, thickness, animation)
·Carrier Label customization(placement, text)
·Clock customization(show clock, show seconds, alignment, ampm, date, date style, date position, date format)
·Network traffic meter options(enable, display units, update interval, hide arrows, auto hide, inactivity threshold)
·Statusbar icon blacklist
·Double tap on statusbar to sleep
·Status bar brightness control
·Status bar notification count
·Status bar bluetooth battery meter toggle

## Navigation Bar
·Navbar toggle and Height/width options
·Navigation bar tuner
·Pixel navbar animation toggle
·Ability to enable one handed mode
·Ability to enabe double tap to sleep
·Longpress back to kill
·Configurable longpress back to kill timeout

## Hardware keys
·Custom key binding
·Backlight control
·Backlight brightness
·Backlight on only when buttons pressed
·Pocket Judge (disable screen and keys while light sensor blocked)
·Accidental touch protection (disable keys while touching screen)

## PowerMenu
·Option to disable on secure lock
·Add/remove (reboot, screenshot, screen-record, torch, airplane mode, user switcher,settings shortcut, search, voice search, lock now, sound panel)

## Volume Rocker
·Volume keys control media volume
·Volume key wake
·Volume key music control
·Volume key orientation swap
·Volume key keyboard cursor control
·Volume up and power action (screen record/selectable screenshot)
·Volume down to enter do not disturb
·Volume up to exit do not disturb
·Do not disturb volume panel switch
·Volume steps customization

## Display
·Expanded desktop options
·Option to enable/disable wake on plug
·3 finger swipe for screenshot toggle
·Battery and Notification LED controls

## Media & Notifications
·Ability to turn off vibration when double tapping power button for camera
·Power notification controls
·Peeking notification option(on/off, timeout, snooze length)
·Low battery notification toggle

## Miscellaneous
·Ability to enable app icon on toast
·Force enable or disable scrolling cache
·Incall vibration options
·Much, much more!