---
title: zipfile 压缩与解压缩
date: 2023-10-31 15:23:46
categories:
- Python学习与实践
- 学习总结
---

# 简介

zip格式编码的压缩和解压缩。

# 压缩

```python
import os,shutil

# 获取需要打包的文件列表
file_list = os.listdir(input())
# 创建一个 ZIP 压缩文件
with zipfile.ZipFile('example.zip', 'w') as zipf:
# 添加文件到压缩文件
        for file in file_list:
            zipf.write(file)
```

# 读取压缩包中的文件信息

```python
    
import zipfile

with zipfile.ZipFile('example.zip', 'r') as zipf:
    file_list = zipf.namelist()
```

# 解压

```python
import zipfile

with zipfile.ZipFile('example.zip', 'r') as zipf:
    zipf.extractall('path')  # 将文件解压缩到指定目录
```