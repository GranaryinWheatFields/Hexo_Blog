---
title: tkinter.filedialog
date: 2023-10-31 15:23:46
categories:
- Python学习与实践
- 学习总结
---

# 简介

`tkinter.filedialog` 模块提供了与文件和文件夹对话框有关的函数，用于在 GUI 应用程序中让用户选择文件和文件夹。以下是一些常用的 `tkinter.filedialog` 函数：
让我们更详细地了解 `tkinter.filedialog` 模块中的每个主要函数：

### 1. `askopenfilename`

```python
from tkinter import filedialog

file_path = filedialog.askopenfilename(title="Select a file", filetypes=[("Text files", "*.txt"), ("All files", "*.*")])
```

- **`title`：** 对话框标题。
  
- **`filetypes`：** 可选文件类型，以元组列表的形式提供。每个元组包含两个值：文件类型的描述和对应的文件扩展名。用户只能选择指定类型的文件。

- **返回值：** 所选文件的路径。

### 2. `askopenfilenames`

```python
from tkinter import filedialog

files = filedialog.askopenfilenames(title="Select files", filetypes=[("Text files", "*.txt"), ("All files", "*.*")])
```

- **`title`：** 对话框标题。
  
- **`filetypes`：** 可选文件类型，以元组列表的形式提供。每个元组包含两个值：文件类型的描述和对应的文件扩展名。用户可以选择多个文件。

- **返回值：** 所选多个文件的路径，以元组形式返回。

### 3. `asksaveasfilename`

```python
from tkinter import filedialog

file_path = filedialog.asksaveasfilename(defaultextension=".txt", filetypes=[("Text files", "*.txt"), ("All files", "*.*")])
```

- **`defaultextension`：** 如果用户未指定扩展名，使用的默认扩展名。
  
- **`filetypes`：** 可选文件类型，以元组列表的形式提供。每个元组包含两个值：文件类型的描述和对应的文件扩展名。

- **返回值：** 用户选择的文件路径用于保存。

### 4. `askdirectory`

```python
from tkinter import filedialog

folder_path = filedialog.askdirectory(title="Select a folder")
```

- **`title`：** 对话框标题。

- **返回值：** 所选文件夹的路径。

