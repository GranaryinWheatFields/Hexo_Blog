---
title: 在文件中寻找特定的元素并保存
date: 2023-11-07
categories:
- Python学习与实践
- 脚本
---

# 需求

遍历文件中的内容，将带有 "id=" 的行内容全部找到写到一个txt文件中。

# 代码


```python

file_input = r"xxx"
file_output = r"xxx/list.txt"
#边读边写
with open(file_input ,"r",encoding="utf-8") as file1, open(file_output,"w",encoding="utf-8") as file2:
    for line in file1:
        if "id=" in line:
            file2.write(line)

```
