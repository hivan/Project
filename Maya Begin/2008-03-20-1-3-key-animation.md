---
layout: post
title: 第一章 第三节 关键帧动画
categories:
- Maya
tags:
- key
- Maya
- 开始maya吧
- 第一章
published: true
comments: false
---
<p><!--more-->
<a href="http://hivan.me/2008/03/20/begin-maya.html" target="_blank">回章目录选择</a></p>

<p><a href="http://hivan.me/2008/03/20/first-maya-animation.html" target="_blank">回节目录选择</a>
<h6>本节概述</h6>
熟悉了Maya动画的开发环境之后，本节用实例讲解如何在Maya中使用关键帧来制作动画。
<h6>理解关键帧动画</h6>
动画是创建和编辑物体的属性随时间变化的过程。关键帧是一个标记，它表明物体属性在某个特定时间上的值。用户通过设置关键帧来描述物体的属性在动画过程中如何变化。设置关键帧包括以下几个步骤：</p>

<p>1． 在时间线(Timeline)中，改变当前时间到需要设置关键帧的位置上。</p>

<p>2． 设定物体属性的数值。</p>

<p>3． 设置关键帧。</p>

<p>在效果上，设置关键帧相当于在特定时间上创建属性的快照。</p>

<p>有几种方式可以为一个属性设置关键帧：</p>

<p>l 使用Animate 菜单中的命令来设置关键帧。</p>

<p>l Path animation（路径动画）使用3D 曲线来设置动画物体的方向。</p>

<p>l 使用属性编辑器和通道盒中的菜单命令来为显示的属性设置关键帧。</p>

<p>l 用户可以使用键盘快捷键来为变换节点属性设置关键帧。</p>

<p>l 使用Graph Editor（图表编辑器）可以为已有动画设置和编辑关键帧。</p>

<p>l 使用Dope Sheet（关键帧列表）可以为已有动画设置和编辑关键帧。
<h6>设置关键帧的方法</h6>
<h6>菜单命令设置关键帧</h6>
1 选择要设置关键帧的物体。</p>

<p>2 选择Animate &gt; Set Key 命令。</p>

<p>Maya 会根据Set Key 命令的选项创建关键帧。
<h6>快捷键设置关键帧</h6>
设置关键帧的快捷键如下：</p>

<p><strong>S</strong><strong>： </strong>如同执行Animate &gt; Set Key 命令，创建关键帧。</p>

<p><strong>Shift-W</strong><strong>： </strong>为移动属性设置关键帧。</p>

<p><strong>Shift-E</strong><strong>： </strong>为旋转属性设置关键帧。</p>

<p><strong>Shift-R</strong><strong>： </strong>为缩放属性设置关键帧。
<h6>自动设置关键帧</h6>
当用户改变当前时间和属性数值时，Auto Key（自动设置关键帧）功能会为属性自动设置关键帧。当用户使用自动设置关键帧时，属性上必须已有一个关键帧。</p>

<p>1 在范围滑块上打开Auto Key 按钮。</p>

<p>2 为物体的某个属性设置关键帧。</p>

<p>3 在时间滑块上选择一个新的时间。</p>

<p>4 改变上面设置关键帧的属性数值。</p>

<p>Maya 会为属性创建一个关键帧。通过重复上面的步骤，用户可以自动创建其它的关键帧。
<h6>保持当前关键帧（Holding current keys）</h6>
1 在范围滑块上打开Auto Key 按钮。</p>

<p>2 为物体的某个属性设置关键帧。</p>

<p>3 在时间滑块上选择一个新的时间。</p>

<p>4 选择Animate &gt; Holding current keys 命令。</p>

<p>使用Hold Current Keys 命令可以在当前时间为物体所有已动画属性设置关键帧。此命令经常与Auto Key 功能一起使用，因为Auto Key 功能只能为改变数值的属性设置关键帧。而Holding current keys命令可以为没有改变数值的动画属性在当前时间也设置关键帧。
<h6>在属性编辑器中设置关键帧</h6>
用户可以编辑和动画属性编辑器中的属性。如果要设置关键帧，在属性盒或属性名称上右击，在弹出菜单中选择Set Key 命令。对于不能设置关键帧的属性，此菜单是无效的。如图1.3.1所示</p>

<p><a href="http://www.flickr.com/photos/95019520%40N00/2347446882/"><img src="http://farm3.static.flickr.com/3289/2347446882_9877aecda6.jpg" border="0" alt="image001" /></a></p>

<p>图1.3.1
<h6>设置受控制帧（Breakdowns）的方法</h6>
受控制帧（Breakdowns）是一种特殊的关键帧，它与临近关键帧在时间上保持一定的比例关系及时保持相临关键帧之间的比例关系。使用受控制帧可以只调整动画的时间，而保持属性值不变。受控制帧在时间滑块上是绿色的标记，而在图表编辑器中是绿点。</p>

<p>对没有临近关键帧的受控制帧，可认为其不受限制。这时，受控制帧在很大程度上和关键帧相似，如放置、编辑和移动操作，而且具有可编辑的切线。当一个或多个受控制帧受关键帧限制时，受控制帧能及时修改它们的位置，反映与关键帧时间位置的位置关系。
<h6>创建受控制帧(Breakdowns)</h6>
l 使用Animate &gt; Set Breakdown 命令可创建受控制帧。此命令的选项设置与Animate &gt; Set Key - 命令的选项设置相同。</p>

<p>l 用鼠标右键单击时间滑块上的关键帧标记，在弹出菜单中选择Keys &gt; Convert to Breakdown，可以将关键帧转化为受控制帧。</p>

<p>l 在图表编辑器中，动画曲线上的所有关键帧都可以转化为受控制帧，在图表编辑器中选择动画属性（或通道），然后选择Keys &gt; Convert to Breakdown。</p>

<p>l 在时间滑块上，也可将受控制帧转化为正常关键帧，在时间滑块上的关键帧标记处右击或者选择某范围的关键帧，并且选择Keys &gt; Convert to Key。</p>

<p>l 在图表编辑器中，也可将动画曲线上所有“受控制帧”变换为关键帧，在图表编辑器中选择已动画的属性（或通道），选择Keys &gt; Convert to Key 命令。
<h6>添加中间帧（Inbetweens）</h6>
中间帧提供了一种方式，它通过增加或去除一帧或一个时间单位来调整动画时间。关键帧和“受控制帧”仍然保持其切线特征，使现有的动画曲线变化最小。</p>

<p>使用关键帧编辑菜单（在时间滑块上右击）选择Keys &gt; Add Inbetween 命令，在当前时间处插入一个中间帧。在图表编辑器使用Keys &gt; Add Inbetween 命令，在当前时间插入一个中间帧。</p>

<p>使用Keys &gt; Remove Inbetween，在当前时间去除一个Inbetween。在去除中间帧时，关键帧之间的空间会减少。这有可能会引起关键帧的冲突，产生意想不到的后果。</p>

<p>使用Add Inbetween 命令将导致动画的关键帧在当前时间向前移动一个时间单位。</p>

<p>使用Remove Inbetween 命令将导致动画的关键帧在当前时间向后移动一个时间单位。
<h6>制作小球弹跳的动画（一）</h6>
小球弹跳动画是每个学习动画的人必修的一课，虽然看起来简单，但是涵盖了动画规律的各个方面，包括关键帧(Key)、时间的掌握（Timing）、间距的掌握(Spacing) 、重量、形变等重要概念。小球弹跳动画对于学习动画的人来讲，就相当于达芬奇画的鸡蛋一样重要，你会从中获得很多乐趣，而你的动画之路也由此展开。动画中的角色可以是任何物体。再简单的物体，如果你给予它“生命”，让它“动”起来，你就是“上帝”了。所以学习动画，可以从最简单的形体开始，逐步熟练自己的动画技巧。</p>

<p>在制作小球弹跳的动画之前，首先要分析小球弹跳的运动规律。小球在行进间跳跃的过程中，在两个方向发生位移的变化，一个是水平方向的运动，另一个是垂直方向的运动。其中小球在垂直方向的运动受到重力的作用，因此在上升过程中是减速运动，在下落过程中是加速运动。因此小球在最高点速度为零，小球在接触地面时速度最大，在受到反弹力的作用下，反向运动。如果不计能量损失，小球弹跳数次的高度将会相同，如果考虑能量损失，小球将会越跳越低，弹跳的间隔也会越来越短。下面在不考虑能量损失的情况下，制作小球弹跳的动画。通过分析可以找出小球运动的关键位置（极端位置）以及过渡位置，如图所示。图中数字表示运动的时间（帧数）。每秒24帧的动画为例，小球每秒钟（24帧）完成一次跳跃。</p>

<p>关键帧（极端姿态）：</p>

<p>小球落地瞬间位置（1、25、49、73）；</p>

<p>小球弹起到最高点（13、37、61）</p>

<p>受控制帧（过渡位置）：</p>

<p>小球在从地面到最高点之间用时一半的位置（7、19、31、43、55、67）如图1.3.2所示</p>

<p><a href="http://www.flickr.com/photos/95019520%40N00/2346616149/"><img src="http://farm3.static.flickr.com/2300/2346616149_7294a06c1d.jpg" border="0" alt="image004" /></a></p>

<p>图1.3.2</p>

<p>实例教程
<h6>1 创建动画的角色。</h6>
在场景中创建一个NURBS球体。然后再创建一个NURBS平面，作为小球碰撞的地面。将平面的TranslateY值设置为-1，ScaleX和ScaleZ分别设置为50。然后分别将小球与平面命名为“ball”和“floor”，如图1.3.3所示。</p>

<p><a href="http://www.flickr.com/photos/95019520%40N00/2346615983/"><img src="http://farm3.static.flickr.com/2388/2346615983_46ae8f457f.jpg" border="0" alt="image005" /></a></p>

<p>图1.3.3
<h6>2 设置小球弹跳的关键帧</h6>
首先，在不考虑能量损失的情况下，制作小球连续跳跃三次动画，这样我们需要在时间线(Timeline)上设置小球的关键帧。</p>

<p>切换到Side视图，在第1帧将通道栏（Channel Box）中将小球的TranslateZ设置为-20，TranslateY设置为0；然后选中通道栏中的TranslateZ和TranslateY属性，如图所示。单击鼠标右键，选择Key Selected命令，设置关键帧。</p>

<p>按F2键进入动画(Animation)模块。打开Auto Key按钮<a href="http://www.flickr.com/photos/95019520%40N00/2347446664/"><img src="http://farm3.static.flickr.com/3168/2347446664_0baa7b8c67.jpg" border="0" alt="image007" /></a>，在第25帧将小球的TranslateZ设置为-10，然后选择菜单中选择Animate &gt; Holding current keys 命令，设置关键帧。在第49帧将小球的TranslateZ设置为0，然后选择菜单中选择Animate &gt; Holding current keys 命令，设置关键帧。在第73帧将小球的TranslateZ设置为10，然后选择菜单中选择Animate &gt; Holding current keys 命令，设置关键帧。播放动画，现在制作了小球沿Z轴正方向匀速前进的动画。如图1.3.4所示</p>

<p><a href="http://www.flickr.com/photos/95019520%40N00/2346615777/"><img src="http://farm3.static.flickr.com/2101/2346615777_cd2ee93b51.jpg" border="0" alt="image009" /></a></p>

<p>图1.3.4</p>

<p>用户可以在工具栏（Shelves）中，创建Holding current keys 命令的快捷方式图标，提高工作效率。在工具栏中增加快捷方式图标的方法如下：选中添加图标的工具栏类别，通常是Animation。然后按住Ctrl+Shift键，选择Animate &gt; Holding current keys 命令，快捷方式图标会添加在工具栏中，如图1.3.5所示。</p>

<p><a href="http://www.flickr.com/photos/95019520%40N00/2347446526/"><img src="http://farm3.static.flickr.com/2374/2347446526_4f8479c634.jpg" border="0" alt="image011" /></a></p>

<p>图1.3.5</p>

<p>在第13帧将小球的TranslateY属性设置为20，选择Holding current keys 命令。在37帧和61帧也将小球的TranslateY属性分别设置为20，并且选择Holding current keys 命令。</p>

<p>播放动画。小球按着时间顺序通过这七个关键帧位置，做波浪运动。但是小球似乎没有受到重力的作用，看起来不像是在跳跃。下面需要调整动画曲线，使小球的跳跃符合运动规律。
<h6>3 使用图表编辑器(Graph Editor)调整动画曲线</h6>
在二维动画中通常使用过渡位置以及中间画法来完成小球的动画规律。在三维动画中，中间动态由三维动画软件的插值算法来完成，因此在设置了小球的关键帧之后。很重要的一个工作就是调节关键帧前后的动画曲线，使角色的动作符合运动规律。</p>

<p>在视图</p>
