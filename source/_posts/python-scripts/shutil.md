---
title: shutil
date: 2023-10-31 15:23:46
categories:
- Python学习与实践
- 学习总结
---

# 简介

shutil库，它作为os模块的补充，提供了复制、移动、删除、等操作。

# 函数及其说明

* shutil.copy(src,dst)
    
    复制文件。

    src表示源文件，dst表示目标文件夹。

* shutil.copytree(src,dst)

    复制文件夹。

    只能移动到一个空文件夹，而不能是包含其他文件的非空文件夹。

* shutil.move(src,dst)

    移动文件/文件夹

* shutil.rmtree(src,dst)

    删除文件夹

    区别os模块中的 remove() 方法只能删除某个文件，mdir() 只能删除某个空文件夹，shutil 模块中的 rmtree() 可以递归彻底删除非空文件夹。