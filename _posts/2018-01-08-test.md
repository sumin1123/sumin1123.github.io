---
layout: blog
archives: true
background-image: https://github.com/sumin1123/sumin1123.github.io/blob/master/style/images/20180110/20180110GSC.png?raw=true
category: 故事
title: 一门编程课是如何改变一个部门的
tags:
- Python
- Senimar
redirect_from:
  - /2018/01/bookindex/
---


# 一门编程课是如何改变一个部门的

## 第一幕 背景

一个叫国产化的部门，在国产化率接近90%的公司里，是没有未来的；一个8人的小部门，在120人大部门里也时常被忽略；许多人都盼望着一份裁员大礼包...

十月底，接到一个任务：在大部门年终研讨会上做分享，时间是6分钟。那时候正好phthon班结业，我突然有个想法：这次能不能酷一点，来个无人演示？于是和彭博开始结对编程。

## 第二幕 坑

进坑、出坑的旅程从此开始...

最初的想法是：把电脑摆上演讲台，我就离开，后面完全靠语音输入命令，从而播放视频。

![](https://github.com/sumin1123/sumin1123.github.io/blob/master/style/images/20180110/20180110plan1.PNG?raw=true)


        入坑：如何语音识别？
        出坑：讯飞语音。
        入坑：讯飞PC版已停止发布
        出坑：出坑论坛找旧版本。
        入坑：讯飞睡眠后，无法唤醒。
        出坑：延长待机时间
        入坑：程序指令都是英文，识别率低
        出坑：输入中文，能识别关键字就可以
        入坑：远离电脑，如何语音输入？离得太近，人还是在舞台上
        出坑：使用长耳机线
        入坑：语音输入，无法输入回车，程序无法执行
        死在坑里：放弃语音输入

几乎放弃的时候，有了第二版简单、粗暴的设计：
    
    * 写2个程序，程序1部署到腾讯云，手机登录web1输入指令，指令保存在数据库中，在web2显示最后一条指令；
    * 程序2运行在本地，爬取web2显示的指令，使用pywin32控制电脑；
    
![](https://github.com/sumin1123/sumin1123.github.io/blob/master/style/images/20180110/20180110plan2.PNG?raw=true)

        入坑：输入法弹出广告
        出坑：删除搜狗输入法
        入坑：如何打开media player？如何打开chrome？如何翻页？如何全屏播放？
        出坑：开启了pywin32的探索
        ......
        最终爬着从坑里出来了

## 第三幕 路演

用了4周进行准备，部门里没有人支持我，他们都建议我放个幻灯片、贴几张图、讲两句结束。那是我已经不能接受凑合这个词了，所有的业余时间都放上去。除了做到了无人演示，路演视频也把一个复杂的电磁储能的技术问题讲得很简单。4周里不仅仅是编程，还新学了ProE机械建模、看了大量产品样本，这是一种思维的转变。

12月8号路演完毕，同事观众傻眼了，截取部门聊天记录、邮件记录；之后是红包扑面而来，最大的红包1200块；不在于多少钱，在于这是外部给我的正反馈。

[优酷视频](http://v.youku.com/v_show/id_XMzIwMjM3NjQxNg==.html?spm=a2h3j.8428770.3416059.1)

![](https://github.com/sumin1123/sumin1123.github.io/blob/master/style/images/20180110/20180110wechart1.PNG?raw=true)
![](https://github.com/sumin1123/sumin1123.github.io/blob/master/style/images/20180110/20180110wechart2.PNG?raw=true)


## 第四幕 之后

开头我说过：一个叫国产化的部门，在国产化率接近90%的公司里，是没有未来的；一个8人的小部门，在120人大部门里也时常被忽略；

这次演讲，可以用惊艳来形容，让大部门老板，想起还有我们这群人。2018年让我们接手850个新项目，这让一些人拿裁员package变得遥遥无期，而另外，一些人看到了自己的创造性，觉得处处可以做得更好，还有一群聪明人在前面等着他。

有时候你做一件事情，并不知道它会给你带来什么影响。

![](https://github.com/sumin1123/sumin1123.github.io/blob/master/style/images/20180110/20180110GSC.png?raw=true)
