Code Style Configs
==================

Code style configuration files.

# checkstyle.xml

## 来源

此文件基于 [Checkstyle](http://checkstyle.org) 提供的实现 [Google Code Style](https://google.github.io/styleguide/javaguide.html) 的配置文件 [google_checks.xml](https://github.com/checkstyle/checkstyle/blob/master/src/main/resources/google_checks.xml) 修改而来。

获取此文件时使用的 Checkstyle 版本为 8.36.2。

## 修改

本文件在原文件的基础上做了一些修改，放宽了一些约束。另有一部分修改是考虑到和的自动化格式工具配合使用时，无法将代码自动格式化到满足约束，所以取消了一部分限制。

### 一般修改

相较与原规则，做出了以下修改：

1. 单行长度限制增加至 120。
2. 右大括号缩进等级和代码块的首行一致。
3. 去除 Javadoc 首行行尾的句号检查。

### 和自动格式化工具冲突导致的修改

1. custom import 修改
2. 关闭 operator wrap

