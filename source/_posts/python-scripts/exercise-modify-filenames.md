---
title: 批量修改文件名
date: 2023-11-01
categories:
- Python学习与实践
- 脚本
---

# 需求

修改某文件夹中的所有.png文件的文件名。

要求都加一个前缀 blog- ，比如 test.png 改为 blog-test.png 。

# 代码

```python
import os

# 输入文件夹路径
path = input("输入文件夹路径: ") 
prefix = "blog_"

# 遍历指定路径下的文件和子文件夹
for root, dirs, files in os.walk(path): 
    for file in files:
        if file.endswith(".png"):  # 检查文件名是否以'.png'结尾
            old_name = os.path.join(root, file)
            new_name = os.path.join(root, prefix + file)
            os.rename(old_name, new_name)  # 重命名文件
            print(old_name + "已修改为: " + new_name)

```