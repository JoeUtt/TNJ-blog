---
title: 谈谈Sketch布局网格（Layout grid)和如何设置
date: 2019-02-07 05:56:26
tags: 
- Sketch
categories: 
- 工作那些事
thumbnail: 'https://xlp-test1.oss-cn-hangzhou.aliyuncs.com/uPic/AHWdDB.jpg'
toc: false
copyright: false
---

最近看了一组关于sketch画板布局（Layout grid)的讨论，总结下经验：

## 响应式网页设计

基本是遵循Bootstrap框架：

- 手机网页4列

- 平板网页8列

- PC站点12列

![pic1](https://xlp-test1.oss-cn-hangzhou.aliyuncs.com/uPic/VMKJv6.png)

间距宽度（gutter width）均为：24px

列数（columns)、偏置（offset）各不相同

总宽（totle width）= 画板（artboard)宽度（px）-2倍的偏置（offset）。如下图 680px的画板(artboard)，布局设置如下：

![pic2](https://xlp-test1.oss-cn-hangzhou.aliyuncs.com/uPic/5UD7CM.png)

<font size="4">[下载sketch示例](https://xlp-test1.oss-cn-hangzhou.aliyuncs.com/uPic/pF8jFr.sketch)</font>

## 手机应用设计

有布局总比没有强，用哪个布局和开发团队去沟通，关键是用哪一个布局。苹果设备有个安全区域，拿iPhone X来讲，Apple自己说有两侧各16px留白，中间区域343px即为安全区域（上留44px，下留34px，这里不管高度），我自己喜欢用**Bootstrap的12列网格和8px的增进**，布局设置如下：

![pic3](https://xlp-test1.oss-cn-hangzhou.aliyuncs.com/uPic/5wDhZh.png)
