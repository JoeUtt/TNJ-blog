---
title: iterm2 美化
date: 2017-05-27 21:20:02
tags: 
- iterm2
categories: 
- 工作那些事
thumbnail: 'https://xlp-test1.oss-cn-hangzhou.aliyuncs.com/uPic/iterm2-1.png'
toc: true
copyright: true
---

## 安装iterm2

## 安装zsh

## 配置zsh

## 配置命令行代理

## 下载安装zsh主题

## 下载安装语法高亮插件

参考 .zshrc 文件

```bash
source /usr/local/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh

# proxy list
alias proxy='export all_proxy=socks5://127.0.0.1:1086'
alias unproxy='unset all_proxy'

# If you come from bash you might have to change your $PATH.
export PATH=$HOME/bin:/usr/local/bin:~/.composer/vendor/bin:$PATH

# Path to your oh-my-zsh installation.
export ZSH=$HOME/.oh-my-zsh

# Set name of the theme to load --- if set to "random", it will
# load a random theme each time oh-my-zsh is loaded, in which case,
# to know which specific one was loaded, run: echo $RANDOM_THEME
# See https://github.com/robbyrussell/oh-my-zsh/wiki/Themes
ZSH_THEME="agnoster"
DEFAULT_USER="joeshi"
```

## 参考

[iterm2和vim美化](https://www.jianshu.com/p/6ff47e388d2d)  
