---
layout: post
title: "git 使用总结"
date: 2020-01-13 
description: "git"
tag: git
---
# git 使用总结  

## １、更改git commit 默认编辑器GNU nano为vim  
* 方法１
```
git config --global core.editor vim
```
* 方法２
编辑~/.gitconfig文件, 在core中添加editor = vim。
* GNU nano 使用
```
ctrl + o 回车　保存
ctrl + x 退出
```