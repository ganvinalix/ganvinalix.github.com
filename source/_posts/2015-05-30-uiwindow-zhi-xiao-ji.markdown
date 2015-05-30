---
layout: post
title: "UIWindow 之小记"
date: 2015-05-30 10:41:18 +0800
comments: true
categories: 
---
#UIWindow的level
UIWindowLevel 是控制window显示层级的关键，level的值设置的越高，那么其展示的越定层
#UIWindow的keyWindow
keyWindow,是和系统交互的，如接收键盘和其他费触摸事件等
，原则上是只有一个window与用户交互，但不代表就只存在一个window。Alert也是一个window。我们可以设置makeKeyWindow或者resinKeyWindow方法来将自己创建的window设置成为一个keyWindow。
