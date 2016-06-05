## 前言

为了适应互联网技术的发展，Adobe公司也全新更新了自己的产品线，其中一个重大的更新就是Flash这个产品了。在互联网技术飞速发展的今天，Flash越来越式微，况且在移动设备上，Flash也越来被唾弃。

随着canvas、svg、webGL等动画技术日益成熟，flash并不是唯一的作动画的选择。

Adobe公司也意识到了这个问题，在2016年年初到时候，全新推出了flash的产品线。原先的flash cc更名为Animate CC，支持canvas、svg以及webGL等互联网标准格式的输出。也就是说，现在使用Animate CC软件可以输出标准的canvas等动画格式的输出。

Adobe公司可能也是希望能复制当初Flash的辉煌，能不能重现flash往日的荣耀，这个还不好说。

不过这段时间，试用了下Animate CC，发现使用它来做动画确实不错。毕竟在动画软件领域积累了这么多年的经验，瘦死的骆驼比马大。

## 时间轴概念

在Animate CC中，首先要明白时间轴的概念。

时间轴是我们创作动画时使用层和帧组织和控制动画内容的窗口，层和帧中的内容随时间的改变而发生变化，从而产生了动画。时间轴主要由层、帧和播放头组成。 

动画是由一格一格的帧构成，通过“视觉暂留”效应使人产生“动”的错觉，而帧就是影像动画中最小单位的单幅影像画面，相当于一格镜头。 

一帧就是一副静止的画面，连续的帧就形成动画，如电视图象等，而flash的时间轴是控制帧的时间分布，明白地说就是控制各个帧在不同时间展现的内容，等到播放的时候，这些帧就会按照你将它们分布在时间轴上的先后顺序产生动画效果。这就是所谓的“帧动画”了。

## FPS

接下来聊聊FPS。FPS全称是：

**FPS**：**Frame Per Second**，翻译过来是每秒的帧数。

也就是说帧数就是在1秒钟时间里传输的图片的量，也可以理解为图形处理器每秒钟能够刷新几次，通常用fps（Frames Per Second）表示。每一帧都是静止的图象，快速连续地显示帧便形成了运动的假象。高的帧率可以得到更流畅、更逼真的动画。每秒钟帧数 (fps) 愈多，所显示的动作就会愈流畅。

详细的一些关于FPS可以去这个[地址](https://www.zhihu.com/question/21081976)看看。

而在Animate CC中，默认的FPS是24，也就是一秒钟播放24帧以形成动画效果。

明白了一些基本的动画原理，就可以开工了。

## 实战

本书的第一个实战是一个简单的矢量动画，很经典的弹球动画。

用到了Animate CC中的形状、自由变形两个工具。一些基本的操作建议去买书看看，太多了，不写了。

到这里才明白，写书是多么的一个体力活，大家错支持支持正版吧。

**写书真不容易**。

最终如下图所示：

![](http://ww4.sinaimg.cn/large/0060lm7Tgw1f4k7kbqsn0g30f90b7dg3.gif)














