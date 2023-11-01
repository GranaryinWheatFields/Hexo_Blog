---
title: 数组对比
date: 2023-11-01
categories:
- Python学习与实践
- 脚本
---

# 需求

对比两个列表，找到两个列表中不一样的部分。

其中一个列表是固定的，另一个列表需要每次遍历文件和文件夹。

# 代码

```python
import os

# 获取当前工作目录下的文件和文件夹列表
list_1 = os.listdir(os.getcwd())

# 预定义要比较的文件和文件夹列表
list_2 = [".vscode", "_static", "_templates", "conf.py", "make_file_docx.py", "make_file_html.py", "test.py"]

# 使用对称差异运算符（^）来找出两个列表之间的不同项
different_folder_list = list(set(list_1) ^ set(list_2)

if len(different_folder_list) != 0:
    for different_folder in different_folder_list:
        print(different_folder)  # 打印不同的文件和文件夹
else:
    print("内容一致")  # 两个列表完全一致

```

```python
# 使用交集操作（&）可以找出两个列表之间的相同项
common_folder_list = list(set(list_1) & set(list_2)
```