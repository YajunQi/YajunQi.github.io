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
* 查看某人的提交记录
````
git log --author="kun.yi"
````
* 查看版本之间的diff
````
git diff ai5/master --stat board/app/appd/
git diff ai5/master board/app/mcud/
````
* 清除master
````
git clean -dfx
````
* 查看log文件之间的不同
````
git log --stat
````
* 切换到某个提交
````
git checkout d12c06c66c56026a773936ceef59b8893d1e3395
````
* 创建分支
```
git checkout -b release-alpha-test
```
* merge
```
git branch -a
git fetch changjun
git branch -a
git merge changjun/mcu-redesign
```
* 拉取本地不存在的远端分支
```
git checkout -b new_branch origin/new_branch
```
* pull 本地库到远端
```
git pull origin 本地分支
```