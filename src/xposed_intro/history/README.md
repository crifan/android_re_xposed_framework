# Xposed发展历史=各种版本

## 概述

* 早期`Android 2.3 ~ 8.1`的：**Xposed**
* 后来`Android 8.0 ~ 11`的：**EdXposed**
* 最新`Android 8.1 ~ 13`的：**LSPosed**

## 详解

* 最早：`Xposed` = `旧版Xposed` = `OG Xposed`
  * 支持Android版本：`Android 2.3` ~ `Android 8.1`
* 后来：`EdXposed`
  * 支持Android版本：`Android 8.0` ~ `Android 11`
    * 已停止维护，不再支持`安卓11+`的版本
  * 主页
    * https://edxp.meowcat.org
  * Github
    * EdXposed
      * https://github.com/ElderDrivers/EdXposed
        * A Riru module trying to provide an ART hooking framework (initially for Android Pie) which delivers consistent APIs with the OG Xposed, leveraging YAHFA (or SandHook) hooking framework, supports Android `8.0 ~ 11`
    * EdXposedManager
      * https://github.com/ElderDrivers/EdXposedManager
* 最新：`LSPosed`
  * 支持Android版本：`Android 8.1` ~ `Android 13`
    * 支持最新的`Android 13`
  * Github
    * https://github.com/LSPosed/LSPosed
      * A Riru / Zygisk module trying to provide an ART hooking framework which delivers consistent APIs with the OG Xposed, leveraging LSPlant hooking framework
  * 官网
    * https://lsposed.org
      * 除了LSPosed的下载地址：
        * https://github.com/LSPosed/LSPosed/releases
      * 之外，啥都没有
        * 或者说：只有一个额外的：（Magisk的MagiskHide替代品的）Shamiko插件 的下载地址
          * https://github.com/LSPosed/LSPosed.github.io/releases
