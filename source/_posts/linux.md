---
title: linux常用命令
date: 2025-08-06 14:40:48
cover: /img/img.jpg
categories:
  - linux

---
# Linux 常用命令汇总

本文档总结了一些常用的Linux命令及其用法。

## 文件复制操作

### 复制整个目录
```bash
cp -r /mnt/e/linux/dir1 .
```
把目录`/mnt/e/linux/dir1`及目录下面所有的文件复制到当前目录中

### 只复制目录中的文件
```bash
cp -r /mnt/e/linux/dir1/* .
```
只复制目录下面的文件，而不是复制整个的目录

### 移动文件/目录
```bash
mv -r /mnt/e/linux/dir1 .
```
把`cp`换成`mv`之后就变成了剪切操作

## 文件查找

### 查找指定文件
```bash
find /mnt/e/linux -name test.json
```
在指定路径中查找特定文件

### 按文件扩展名查找
```bash
find /home/user1 -name "*.bin"
```
查找`.bin`结尾的文件

## 文件权限管理

### 添加可执行权限
```bash
chmod +x aaa.sh
```
给文件`aaa.sh`添加可执行权限
- `+` 代表增加权限
- `-` 代表移除权限

### 设置完整权限
```bash
chmod 777 file1
```
给文件`file1`设置可读、可写和可执行的权限
- r(读) = 4
- w(写) = 2  
- x(执行) = 1

### 更改文件所有者
```bash
chown user1 file1
```
改变文件`file1`的所有者为`user1`

## 总结

这些是Linux系统中最常用的文件操作命令，掌握这些命令可以帮助你更高效地管理文件和目录。

