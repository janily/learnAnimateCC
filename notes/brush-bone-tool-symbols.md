## 骨骼动画工具

在Animate CC中，骨骼动画工具非常实用。

开始之前，还是先来了解下骨骼动画以及Animate CC中骨骼动画的相关概念。

骨骼动画：仿照“真实”的骨骼结构，建立一个节点树，每个节点算是一个骨骼的关节，然后在这些关节上指定关键帧，通过一些计算来生成中间帧。所谓FK和IK，都是计算中间帧节点位置的方法。3D骨骼需要两个步骤，一是rigging（绑骨），就是建立一个骨骼框架，而是skinning（贴皮？），就是把3D模型对应到骨骼框架上。2D骨骼其实是一个比较模糊的概念，可以按照3D这个流程走，进行绑骨和贴皮，但是很多游戏所谓的2D骨骼并没有一个严谨的骨骼结构（通常也没有必要），而是直接在“皮”上做动画。在骨骼基础之上，用一些拉伸变形的非骨骼技巧也是非常常见的。

在上面的骨骼动画概念中提到来两个概念，及所谓FK和IK：

FK（Forward Kinematics，翻译成正向运动？）：就是直接指定节点的位置，然后简单的计算中间帧位置。

IK（Inverse Kinematics，翻译成反向运用？）：正向的指定节点位置太麻烦了，根据一些简单的观察，大家（搞机器人和计算机图形的）发现典型的人体运动是有规律的，关节弯曲的时候会以一个尽量“省力”的方法。IK就是定义一个“省力的标准”，自动生成中间节点的位置。比如一个动画师在调手臂的动画，用FK，他需要分别指定手关节和肘关节两个节点的骨骼位置和方向，用IK，他只需要放置手关节的节点，动画工具会根据算法自动生成肘关节的位置和方向。因为大部分IK的实现是基于经验的简单算法，所以通常会有一些死角和不可用的情况。想准确的计算骨骼中间节点位置需要模拟肌肉和骨骼的biomechanics，在一般的动画软件中做不大，也没多大必要。

上面这两个说明直接来自知乎[这里](https://www.zhihu.com/question/24496292)。

简单来说 IK动画就是反向动力学，就是子骨骼节点带动父骨骼节点运动。比如跳街舞的少年用手撑着身体在地上转圈，手就是子骨骼，胳膊身体就是它的父骨骼，这时运动手就需要带动胳膊身体来移动。

在Animate CC中使用骨骼动画非常简单。

1、在工具面板栏中选择骨骼动画工具

2、在你要使用骨骼动画的对象上，点击并且拖拽然后松开再点一下，如此反复就可以把对象连接起来如下图所示：

![](http://ww1.sinaimg.cn/large/0060lm7Tgw1f4sst5y6ikj307j07r0t6.jpg)

3、然后插入几个关键帧，在每一个关键帧上拖拽骨骼的关节点，就可以做出骨骼动画。一般在一些人物动画上用的比较多。

## 笔刷

在Animate CC中新增一些艺术笔刷工具，作为一个动画设计工具，我觉的这个有点鸡肋。

![](http://ww3.sinaimg.cn/large/0060lm7Tgw1f4st41yva6j30s90ee41n.jpg)

## 元件

元件是指在Flash中创建且保存在库中的图形、按钮或影片剪辑，可以自始至终在影片或其他影片中重复使用，是flash动画中最基本的元素；

影片剪辑元件——可以理解为电影中的小电影，可以完全独立于主场景时间轴并且可以重复播放。

按钮元件——实际上是一个只有4帧的影片剪辑，但它的时间轴不能播放，只是根据鼠标指针的动作做出简单的响应，并转到相应的帧。通过给舞台上的按钮实例添加动作语句而实现flash影片强大的交互性。

图形元件——是可以重复使用的静态图像，或连接到主影片时间轴上的可重复播放的动画片段。图形元件与影片的时间轴同步运行。

#### 区别

影片剪辑元件、按钮元件和图形元件最主要的差别在于，影片剪辑元件和按钮元件的实例上都可以加入动作语句，图形元件的实例上则不能；

影片剪辑元件在场景中敲回车测试时看不到实际播放效果，只能在各自的编辑环境中观看效果，而图形元件在场景中即可适时观看，可以实现所见即所得的效果。

影片剪辑中可以勘套另一个影片剪辑，图形元件中也可以勘套另一个图形元件，但是按钮元件中不能勘套另一个按钮元件；三种元件可以相互勘套。





