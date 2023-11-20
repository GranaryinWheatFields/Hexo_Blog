---
title:  在文件中寻找特定的元素并保存（2）
date: 2023-11-20
categories:
- Python学习与实践
- 脚本
---

# 需求

此篇是[在文件中寻找特定的元素并保存（1）](../exercise-search-id.md)的需求迭代。

1 遍历文件中的内容，将带有 xref:xxx.adoc[] 的行内容全部找到；

2 对行内容做二次处理，只保留 xref:xxx.adoc[] 这个字段。


# 代码

```python

file_input = r"xxx"
file_output = r"xxx/list.txt"
with open(file_input ,"r",encoding="utf-8") as file1, open(file_output,"w",encoding="utf-8") as file2:
    for line in file1:
        if "xref:" in line:
            index_start = line.find("xref:")
            index_end = line.find(".adoc")
            line = line[index_start:index_end + 5]
            file2.write(line)
```


