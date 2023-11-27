---
title: 从文件中读取一个变量
date: 2023-11-27
categories:
- Python学习与实践
- 脚本
---

# 需求

将变量写在一个文件中，脚本每次读取文件中的变量进行处理。

# 代码


```python

# 读取文件
file_path = 'input.txt'

try:
    with open(file_path, 'r') as file:
        # 从文件中读取变量
        variable_to_process = file.read()
        print(f"从文件中读取的变量值为: {variable_to_process}")

        # 在这里可以对变量进行处理
        # ...

except FileNotFoundError:
    print(f"找不到文件: {file_path}")
except Exception as e:
    print(f"发生了错误: {e}")


```
