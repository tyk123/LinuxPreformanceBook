在我们开始前，先来浏览一下Linxu操作系统是怎样控制任务来完成与硬件资源交互的。性能调优是一项富有挑战性的工作，它需要对硬件、操作系统和应用有非常深入的了解。但如果性能调优很简单，那么我们所要探究的配置参数就可以直接硬编码到韧体或操作系统中了，你今天就不会看到本文了。然而正如图1-1所示，服务器性能会受到多种因素的影响。

图1-1：不同元件交互示意图

如果一个有20000名用户的数据库服务器，却只拥有一个单IDE驱动器，这样的I/O子系统你可能花几个星期的时间都无法有效的调优。为了能带来更好的性能，通常作法是更换一个新的驱动器或者将你的应用升级。正如我们之前所讨论的，请在头脑中保持对系统性能的整体印象。了解操作系统管理资源的方法，可以帮助我们在各种各样的应用情境中找出哪个子系统需要调优。

注释：本文主要讨论Linux操作系统的性能。

本章内容包括：

1.1 Linux进程管理

1.2 Linux内存管理

1.3 Linux文件系统

1.4 硬盘I/O子系统

1.5 网络子系统

1.6 了解Linux性能量度