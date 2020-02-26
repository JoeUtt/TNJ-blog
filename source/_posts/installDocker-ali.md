---
title: 阿里云Ubuntu安装Docker
date: 2017-05-31 20:10:02
tags: 
- 阿里云
- Ubuntu
categories: 
- 工作那些事
thumbnail: 'https://xlp-test1.oss-cn-hangzhou.aliyuncs.com/uPic/Tqp2CV.png'
toc: true
copyright: true
---

这里以Ubuntu下安装Docker为例介绍如何安装Docker。
Docker要求Ubuntu操作系统为64位，并且Lunix内核版本至少是3.10。您需要先确认操作系统位数和内核版本符合要求。
如果您的系统符合要求，则可以接着进行操作。

## 首先，进入Ubuntu系统打开Terminal，更新包管理器，安装程序包

```bash
sudo apt-get update$ sudo apt-get install linux-image-generic-lts-trusty
sudo reboot
```

## 然后，在Ubuntu上安装Docker

获取root权限

```bash
su root
```

确认是否安装了文件传输工具

```bash
which curl
```

如果没有安装，则使用命令安装

```bash
sudo apt-get update
sudo apt-get install curl
```

## 安装curl后，使用curl获取最新的Docker

```bash
curl -sSL http://acs-public-mirror.oss-cn-hangzhou.aliyuncs.com/docker-engine/internet | sh -
```

注：如果您使用的是阿里云ECS，可以改为使用下面命令，通过内网下载。

```bash
curl -sSL http://acs-public-mirror.oss-cn-hangzhou.aliyuncs.com/docker-engine/intranet | sh -
```

验证Docker是否安装成功。

```bash
sudo docker run hello-world
```
