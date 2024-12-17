# 安卓逆向调试：XPosed框架

* 最新版本：`v3.3.1`
* 更新时间：`20241217`

## 简介

介绍用于安卓破解的辅助工具：Xposed框架；先是Xposed框架简介，Xposed发展历史，从Xposed到EdXposed，再到LSPosed；然后介绍背景知识，包括Riru、Zygisk等；再介绍类XPosed框架的VirtualXposed、太极、LSPatch；接着介绍具体如何安装Xposed、EdXposed、LSPosed；其中包括EdXposed常见问题；LSPosed的相关日志、打开LSPosed的app、LSPosed的界面和功能、Shamiko模块；如何具体使用XPosed；以及常见的XPosed的插件模块，包括JustTrustMe，砸壳导出dex的FDex2和dumpdex，app可调试的Xdebuggable和XAppDebug，以及GravityBox；然后介绍如何开发XPosed插件，包括先是用AS新建一个安卓普通app项目，再去改动增加Xposed的配置，写Xposed插件的hook代码，编译和安装Xposed插件即普通安卓apk到安卓手机，然后确认Xposed插件是否安装成功和被正常识别，然后测试Xposed插件是否生效是否能输出log日志；以及贴出Xposed插件的demo项目源代码。最后整理Xposed相关心得；

## 源码+浏览+下载

本书的各种源码、在线浏览地址、多种格式文件下载如下：

### HonKit源码

* [crifan/android_re_xposed_framework: 安卓逆向调试：XPosed框架](https://github.com/crifan/android_re_xposed_framework)

#### 如何使用此HonKit源码去生成发布为电子书

详见：[crifan/honkit_template: demo how to use crifan honkit template and demo](https://github.com/crifan/honkit_template)

### 在线浏览

* [安卓逆向调试：XPosed框架 book.crifan.org](https://book.crifan.org/books/android_re_xposed_framework/website/)
* [安卓逆向调试：XPosed框架 crifan.github.io](https://crifan.github.io/android_re_xposed_framework/website/)

### 离线下载阅读

* [安卓逆向调试：XPosed框架 PDF](https://book.crifan.org/books/android_re_xposed_framework/pdf/android_re_xposed_framework.pdf)
* [安卓逆向调试：XPosed框架 ePub](https://book.crifan.org/books/android_re_xposed_framework/epub/android_re_xposed_framework.epub)
* [安卓逆向调试：XPosed框架 Mobi](https://book.crifan.org/books/android_re_xposed_framework/mobi/android_re_xposed_framework.mobi)

## 版权和用途说明

此电子书教程的全部内容，如无特别说明，均为本人原创。其中部分内容参考自网络，均已备注了出处。如发现有侵权，请通过邮箱联系我 `admin 艾特 crifan.com`，我会尽快删除。谢谢合作。

各种技术类教程，仅作为学习和研究使用。请勿用于任何非法用途。如有非法用途，均与本人无关。

## 鸣谢

感谢我的老婆**陈雪**的包容理解和悉心照料，才使得我`crifan`有更多精力去专注技术专研和整理归纳出这些电子书和技术教程，特此鸣谢。

## 其他

### 作者的其他电子书

本人`crifan`还写了其他`150+`本电子书教程，感兴趣可移步至：

[crifan/crifan_ebook_readme: Crifan的电子书的使用说明](https://github.com/crifan/crifan_ebook_readme)

### 关于作者

关于作者更多介绍，详见：

[关于CrifanLi李茂 – 在路上](https://www.crifan.org/about/)
