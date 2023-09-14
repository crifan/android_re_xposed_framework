# Xposed简介

* `XPosed`
  * 是什么：本身是一个框架
    * 所以也称：`XPosed框架`
      * =`Xposed Framework`
  * 适用对象：（已root的）安卓手机
  * 作用：可以在XPosed中安装各种插件，实现各种高级功能
    * 引申：常被用来配合破解安卓应用
      * 比如
        * 用`FDex2`砸壳导出`app`的`dex`文件
        * 自己编写`XPosed`hook插件，实现特定功能
  * 前提：需要安卓手机有`root权限`
  * 特点
    * 开源
    * 支持插件
      * 安装插件后，可以实现各种原本很难实现的效果
  * Github
    * https://github.com/rovo89/XposedBridge
      * rovo89/XposedBridge: The Java part of the Xposed framework.
    * Wiki
      * https://github.com/rovo89/XposedBridge/wiki
        * Using the Xposed Framework API · rovo89/XposedBridge Wiki
          * https://github.com/rovo89/XposedBridge/wiki/Using-the-Xposed-Framework-API
  * 最新的变体
    * `EdXposed`
    * `LSPosed`
