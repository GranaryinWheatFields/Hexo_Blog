---
title: os
date: 2023-10-31 15:23:46
categories:
- Python学习与实践
- 学习总结
---


# 简介

os 全称为 operating system，这个模块提供了与操作系统交互的各种函数，我们可以通过这些函数调用计算机底层操作系统的部分功能来快速、高效地管理文件和目录。

此篇文章列举了os模块常见函数及其说明。

# 函数及其说明

* os.getcwd()

    得到当前工作目录，即当前Python脚本工作的目录路径。

* os.listdir()

    返回指定目录下的所有文件和目录名。

* os.remove()

    删除一个文件。

* os.removedirs()

    删除多个目录。

* os.path.isfile()

    检验给出的路径是否是一个文件。

* os.path.isdir()

    检验给出的路径是否是一个目录。

* os.path.isabs()

    判断是否是绝对路径。

* os.path.exists()

    检验给出的路径是否存在。

* os.path.splitext()

    分离扩展名。

* os.path.dirname()

    获取路径名。

* os.path.basename()

    获取文件名。

* os.system()

    运行shell命令。

* os.rename（old， new）

    重命名。

* os.makedirs（r“c：\python\test”）

    创建多级目录。

* os.mkdir（“test”）

    创建单个目录。

* os.stat()

    获取文件属性。

* os.chmod()

    修改文件权限与时间戳。

* os.exit()

    终止当前进程。

* os.path.getsize()

    获取文件大小。

* os.walk()

    这个函数需要传入一个路径作为top参数，函数的作用是在以top为根节点的目录树中游走，对树中的每个目录生成一个由(dirpath, dirnames, filenames)三项组成的三元组。

    其中，dirpath是一个指示这个目录路径的字符串，dirnames是一个dirpath下子目录名（除去“.”和“..”）组成的列表，filenames则是由dirpath下所有非目录的文件名组成的列表。要注意的是，这些名称并不包含所在路径本身，要获取dirpath下某个文件或路径从top目录开始的完整路径，需要使用os.path.join(dirpath, name)。

* os.path.join()

    将多个传入路径组合为一个路径。