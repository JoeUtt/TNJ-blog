---
title: 阿里云Ubuntu安装NodeJS
date: 2017-05-31 20:20:02
tags: 
- 阿里云
- Ubuntu
categories: 
- NodeJS
thumbnail: 'https://xlp-test1.oss-cn-hangzhou.aliyuncs.com/uPic/nNuiqk.png'
toc: false
copyright: true
---

## 执行检查可更新的软件

    ```bash
    apt update
    ```

## 先用普通的apt工具安装低版本的Node

    ```bash
    apt install nodejs
    apt install nodejs-legacy
    apt install npm
    ```

## 更换淘宝源

    ```bash
    npm config set registry https://registry.npm.taobao.org
    ```
    查看是否生效
    ```bash
    npm config list
    ```

## 安装 Node 版本更新工具 N  

    ```bash
    npm install n -g
    ```

## 更新 Node 版本到稳定版

    ```bash
    n stable
    ```

  或者更新到指定版本,如v10.10

    ```bash
    n v10.10
    ```

## 创建软链

    ```bash
    ln -sf /usr/local/n/versions/node/<VERSION>/bin/node /usr/bin/nodejs
    ```

## 查看 Node 版本

    ```bash
    node -v
    ```

## 安装 CNPM

    ```bash
    npm install cnpm -g
    ```
