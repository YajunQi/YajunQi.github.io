---
layout: post
title: "Linux命令学习-常用命令"
date: 2019-08-25 
description: "Linux命令学习-常用命令"
tag: Linux命令学习
--- 
# Linux 命令学习-磁盘空间管理

# alias  
#### 功能：设置命令的別名  
#### 语法：alias [-p][別名][=命令]  
#### 包名称：bash
#### 相关命令：unalias
#### 补充说明：alias 查询当前所有別名，alias及作用于该次登录的作业；若登录自动设置好，.profile(bash)或.cshrc(tcsh） 

| 参数 | 含义|  
| :----| :---- |
| -p |列出当前所有的別名设置|
| 別名|列出指定的別名设置|
|別名=命令名称|设置某个命令的別名|  

###范例：
* 列出当前所有的別名设置
```
# alias 
```  
* 将mkdir命令的別名设为md：  
```
#alias md=mkdir
#alias md
```
* 将ls-al命令的別名设置为dir  
```
# alias dir='ls-al'
```


# cat(concatenate)  
#### 功能说明：  
连接多个文件，并将他们的内容输出到标准输出设备。
#### 语法：  
cat[-AbeEnstTuv][--help][--version][文件 ...]
#### 包名称：  
coreutils
#### 相关命令：  
csplit、cut、head、tac、tail、zcat
* csplit：将一个大文件分割成小的碎片，并且分割后的每个碎片保存成一个文件。
* cut：指定欲显示的文件内容，输出到标准输出设备。
* tac:用于将文件已行为单位反序输出，即第一行最后显示，最后一行先显示。
* tail：用于输入文件中的尾部内容。
* zcat：用于不真正解压缩文件，就能显示压缩包中文件内容的场合。  
####补充说明：  
cat命令会读取指定文件的内容，并输出到标准的输出设备上（例如显示器）。  若不指定任何文件名称，或是指定的文件名为“-”，
则cat命令会从标准输入设备读取数据（例如键盘），然后把所得到的数据输出到输出设备。也运用shell的特殊字符“>”和“>>”,把
多个文件的内容合并成一个文件。

|参数|说明|
|:----|:----|
|-A或--show-all|此参数的效果和同事指定“-vET”参数相同|