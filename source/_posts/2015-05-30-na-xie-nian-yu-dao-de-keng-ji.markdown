---
layout: post
title: "那些年遇到的坑记"
date: 2015-05-30 11:15:45 +0800
comments: true
categories: 
---
#float的坑
1.系统版本判断建议不用float比较如 eg version > 7.1 之类的,推荐按使用compare

	#define IOS4_OR_LATER ( [[[UIDevice currentDevice] systemVersion] compare:@"4.0"] != NSOrderedAscending )

2.uilabel frame的origin值如果有是小数位在非retina的ipad mini的 屏幕上内容模糊。

go on......