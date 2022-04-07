---
title: Apk和Odex的介绍与合并 (含合并工具)
categories:
  - 资源教程
toc: true
abbrlink: 65218
date: 2017-08-24 15:13:23
urlname:
tags:
  - Odex
---
## Odex合并工具- SVADeodexerForArt V5.5（支持安卓7.0）
### From [XDA](https://forum.xda-developers.com/galaxy-s5/general/tool-deodex-tool-android-l-t2972025) 更多版本与信息请前往查看
官方安卓系统本身是apk与dex分离的，但是开发者为了修改、调整一些参数，不得不去对“Framework”和“Apk”进行合并后再去修改！通常我们会使用安卓厨房(Android Kitchen)来合并，不过自从系统升级arm64后，官方已经不能进行合并处理了，不过大神开发了一款专门用来deodex的工具 - SVADeodexerForArt，这是一款Windows下电脑端对官方的Apk和Odex文件进行合并的工具，开发者值得拥有！也是ROMer的必备工具之一，做系统文件的修改和美化少不了它。

**1.** Download for 32-bit systems (**v5.5** from **21-04-2017**): [SVADeodexerForArt_v5-5_32.zip](https://forum.xda-developers.com/attachment.php?attachmentid=4120575&d=1492765409 "Name:  SVADeodexerForArt_v5-5_32.zip")

**2.** Download for 64-bit systems (**v5.5** from **21-04-2017**): [SVADeodexerForArt_v5-5_64.zip](https://forum.xda-developers.com/attachment.php?attachmentid=4120576&d=1492765409 "Name:  SVADeodexerForArt_v5-5_64.zip")
***
# Apk和odex的介绍与合并
>以下文章 《给大家科普一下安卓知识，apk和odex的介绍和合并，很有用哦》 出自 [MIUI](http://www.miui.com/thread-839026-1-1.html) 论坛 ；排版 [Me-1](https://www.me-1.cn)

## APK介绍
***
APK是Android Package的缩写，即Android安装包。APK是类似SymbianSis或Sisx的文件格式。通过将APK文件直接传到Android模拟器或Android手机中执行即可安装。

APK文件其实是zip格式，但后缀名被修改为apk，通过UnZip解压后，可以看到Dex文件，Dex是DalvikVM executes的全称，即Android Dalvik执行程序，并非Java ME的字节码而是Dalvik字节码。

一个APK文件(压缩文件打开可以看到)结构为：

- `mete-INF\`  Jar文件中常可以看到
- `res\ `存放资源文件的目录
- `AndroidManifest.xml`  程序全局配置文件
- `classes.dex Dalvik`字节码
- `resources.arsc` 编译后的二进制资源文件

总结下我们发现Android在运行一个程序时首先需要`UnZip`，然后类似`Symbian`那样直接，和Windows Mobile中的`PE`文件有区别，这样做对于程序的保密性和可靠性不是很高，通过`dexdump`命令可以反编译，但这样做符合发展规律，微软的 `Windows Gadgets`或者说`WPF`也采用了这种构架方式。

在Android平台中`dalvik vm`的执行文件被打包为apk格式，最终运行时加载器会解压然后获取编译后的`androidmanifest.xml`文件中的`permission`分支相关的安全访问，但仍然存在很多安全限制，如果你将apk文件传到`/system/app`文件夹下会发现执行是不受限制的。最终我们平时安装的文件可能不是这个文件夹，而在android rom中系统的apk文件默认会放入这个文件夹，它们拥有着root权限。

## odex文件介绍 
***
细心的网友可能发现Android的ROM中有很多odex文件，相对于 APK中的dex文件而言这个odex有什么作用呢?

如果你仔细观察会发现文件名时一一对应的，同时那些对应的apk文件中没有dex文件。这样做可以使其厂商保证一定的反盗版，因为没有没有dex文件的apk是无法正常安装的，而厂商直接将odex和不完整的apk文件放到手机rom固化到`/system/bin`中可以让一般用户无法正常导出使用。（文/Android开发网）

很多网友可能想到的是合并odex和apk变成apk中包含dex文件的，这样合并后最终apk文件安装在`/data/`中，而rom存放时在` /system/bin`中，所以最终导致了用户可装在Android手机中的软件会变少，占用系统空间。

- ### APK生成 odex文件方法:
1.编译开源GIT上的`build/tools /dexpreopt/dexopt-wrapper`这个，使用`dexopt-wrapper`即可，操作步骤
2.将`dexopt-wrapper`放到`/data/local`目录中
使用adb shell执行linux命令行，使用cd命令进入`/data/local`目录，


    cd /data/local./dexopt-wrapper android123.apk android123.odex


- ### 合并odex和dex的apk 为完整的apk文件
需要用到的工具是smali，一个开源的java处理软件： http://code.google.com/p/smali/downloads/list
 - 下载的baksmali和 smali的jar文件到工作目录
 - 把ROM里面的`core.odex`, `ext.odex`, `framework.odex`, `android.policy.odex`,`services.odex`这5个文件也放在同一目录（也可以放在别的目录，通过设置BOOTCLASSPATH指定，默认就是当前目录）。
 **例：以teeter为例子 (HTC一些Android常常会内置)，ROM里面拿出来的可能是2个文件，teeter.apk + teeter.odex。**
 1、分解odex文件：
`java -jar baksmali-1.2.1.jar -xteeter.odex`
如果没其他问题，会在工作目录生成一个out的目录，里面是分解出来的一些文件。
2、把分解得到的文件变成`classes.dex`：`java -Xmx512M -jar smali-1.2.1.jarout -o classes.dex`，这样得到了一个有用的`classes.dex`文件
3、用WinZip或者WinRAR打开`teeter.apk`文件，把这个`classes.dex `放进去
4、最后再用signapk把最新得到的这个包含`classes.dex`的apk重新签署一下 (Auto Sign签名工具往期的文章里有下载)，就生成一个可以安装的单独APK程序了。
5、签名完成后即可安装使用了