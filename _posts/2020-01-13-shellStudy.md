---
layout: post
title: "shell 脚本学习"
date: 2020-01-13 
description: "linux shell 脚本学习"
tag: linux study
---
## 字符串判断
```
#!/bin/bash

#cat /home/qyj/shell_tset/test.c | grep Mode
#result=$?
#echo $result:
#print the return status value

normal="normalMode"
sleep="sleepMode"

cat_ret()
{
    cat /home/qyj/shell_tset/test.c | grep Mode
}
ret=`cat_ret`

if [ ${ret} == "normalMode" ]; then
    echo $normal
elif [ ${ret} == "sleepMode" ]; then
    echo $sleep
else
    echo "error"
fi    

#echo "State: "$1 # echo the return status value
#echo "ret: "${ret} # echo the return value of cat_ret
```