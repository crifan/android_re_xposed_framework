# Zygisk

## 什么是Zygisk

* Zygisk is a new feature in Magisk that provides a different way of running root apps and modules
  * Instead of running them as root, Zygisk creates a separate environment for these apps to run in. This environment is called the Zygote process, which is a system process in Android that is responsible for launching and managing app processes.
  * The Zygote process is the very first Android OS process that starts when you boot your phone. This is equivalent to the PID 1 process when you start a Linux based computer or server. Magisk allowing Zygisk to run at the boot level means it can have root access without sending that data to your apps.
* Zygisk是Zygote的Magisk
  * 这将在Zygote进程中运行Magisk的一部分，使Magisk模块更强大。
  * 日常使用中，Zygisk运行在Android核心进程Zygote中。
  * 当一个进程在上述拒绝列表中时，Magisk 将清理该进程的内存空间以确保不应用任何修改，而 root 进程仍然可以在没有 Magisk 监督的情况下通过各种技巧将代码注入其他进程
  * 或者我们更加简单的理解，Zygisk就类似1个新的运行环境，此环境相对于之前的Riru存在天壤之别，这也是为什么zygisk和riru不能同时使用的原因。

## Zygisk用途和好处？

* By running root apps and modules in the Zygote process, Zygisk provides several benefits, including improved compatibility, security, and performance. Most importantly, your privacy focused apps like banking apps, Netflix, Google Play Movies etc. will not detect your rooted device and will continue to work like normal.
  * improves compatibility
  * enhances security
  * improve performance
* 引入Zygisk后，传统MagiskHide已经被取消，但是我们可以在面具设置里，打开Zygisk按钮再Zygisk环境下，多出来1个排除列表。
  * 在排除列表进入后，界面非常类似之前的Magisk  Hide功能，通过对排除列表里部分软件打钩，成功对软件实现了ROOT隐藏。
  * 除以上这些打开Zygisk后，我们刷入相关模块后，只需要直接刷入功能模块即可实现。
  * 如LSPosed分riru版和Zygisk版本：
    * Riru版本激活LSP需要刷入riru+lsp两个zip才能实现
    * 而Zygisk版本直接刷1个ZyLSP即可快速激活
      * 操作起来更加简单
