---
title: Drama原型、动效工具实战（一）---- Drama对sketch symbols支持不够好
date: 2019-06-22 22:11:41
tags: 
- Drama.app
categories: 
- 工作那些事
thumbnail: 'https://xlp-test1.oss-cn-hangzhou.aliyuncs.com/uPic/2dpTYb.png'
toc: false
copyright: false
---

⏬[下载文章所用Drama工程](https://xlp-test1.oss-cn-hangzhou.aliyuncs.com/uPic/N4O5cP.drama)

## 导入Sketch文件

- 刚导入完就发现有个巨大问题，和Sketch控件有关：如果在画板里修改Sketch控件里原有的填充图，对不起，Drama只认在控件里的图。

    ![bug1](https://xlp-test1.oss-cn-hangzhou.aliyuncs.com/uPic/OkDXz3.png)

这样一来，似乎又增加了很多工作量 😭

💡解决方法：

1. 如果工程要使用Drama，那少用sketch控件；

2. 等Drama修复这个bug。

- 尽力优化sketch对象，保留重点对象：需要添加动效的对象。否则在Drama里编辑动效会头大... Drama性能也会下降。

    ![mess-objects](https://xlp-test1.oss-cn-hangzhou.aliyuncs.com/uPic/EiijFY.png)

    未做优化的sketch工程里的对象

💡解决方法：

1. sketch不涉及动效的对象切图处理。

2. 优化sketch对象分组，涉及动效的单独拎出来。

- 优化后

    ![optimized](https://xlp-test1.oss-cn-hangzhou.aliyuncs.com/uPic/gHAKSL.png)

- 一番折腾后

    ![final](https://xlp-test1.oss-cn-hangzhou.aliyuncs.com/uPic/yBOAUD.gif)

- 导出

    Drama支持60帧的视频导出，**可以加水印**。有趣的是还支持加特效渲染导出（导出非常慢）。

## 总结

- Sketch工程要提前规划，把需要交互的对象**单独组成一组**。

- 要Drama，Sketch少用控件。（当前版本）

Love you 3000 💗💗
