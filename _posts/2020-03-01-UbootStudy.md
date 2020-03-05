---
layout: post
title: "Uboot 学习总结"
date: 2020-03-01
description: "uboot summary"
tag: linux study
---
# Uboot 学习总结   

```
tftp 0x82000000 AI5-burn-hi3521d-V2.5.0-20200228-9c06ade.bin; sf probe 0; sf erase 0 1E00000; sf write 82000000 0 1E00000
sf - SPI flash sub-system
对spi flash进行操作的命令
uboot中如果支持spi/qspi flash, 那么可以使用sf的erase, read, write命令操作spi flash

sf read用来读取flash数据到内存
sf write写内存数据到flash
sf erase 擦除指定位置,指定长度的flash内容, 擦除后内容全1
```