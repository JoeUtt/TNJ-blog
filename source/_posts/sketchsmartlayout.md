---
title: 什么是 Sketch 智能布局（Smart Layout）？
date: 2019-09-15 15:32:50
tags: 
- Sketch
categories: 
- 工作那些事
thumbnail: 'https://xlp-test1.oss-cn-hangzhou.aliyuncs.com/uPic/vteR05.png'
toc: false
copyright: false
---

`Sketch 58`版本推出了Smart layout，中文叫“智能布局”。主要是针对控件（symblos）的更新。用了几天下来，总结下心得。

## 使用智能布局（Smart Layout)

- 控件（symbols）创建完后，sketch会自动为控件（symbols）创建一个母版（master）和一个实例（instance）。

- 控件创建时的布局（Layout），是指在控件被覆盖层（override）撑开时的方向，横向：左 --> 右，右 --> 左，中间向两边；纵向：上 --> 下，下 --> 上，中间向上下。特别注意下：**如果选择横向布局，文字布局（text layout）要选择自动宽度（Auto Width）；选择纵向布局，文字布局（text layout）要选择自动高度（Auto Height）。**

    ![layout](https://xlp-test1.oss-cn-hangzhou.aliyuncs.com/uPic/WNQqWY.png)

- 控件（Symbols）本身可以组合使用，那同样，组合使用的控件（Symbols）的智能布局（Smart Layout）同样适用。
  
    ![smartlayout](https://xlp-test1.oss-cn-hangzhou.aliyuncs.com/uPic/hlpIAV.png)

## 总结

- 使用控件（Symbols）才能使用智能布局（Smart Layout），即，智能布局（Smart Layout）是为了增强控件（Symbols）功能而推出。

- 可以摆脱一些拖Sketch性能的小插件了。

Love you 3000 💗💗
