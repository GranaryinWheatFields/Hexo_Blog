---
title: 一个选择文件并显示路径的GUI
date: 2023-10-31 15:23:46
categories:
- Python学习与实践
- GUI
---

# 需求

使用 tkinter 创建一个GUI，GUI 分为两部分，其中一个按钮点击后可选择文件，另一个文本显示窗口将显示文件路径。

# 代码

```python

import tkinter as tk
from tkinter import filedialog

# 定义按钮调用的函数，即文件选择
def open_file_dialog():
   file_path = filedialog.askopenfilename() # 使用askopenfilename将返回值赋值给file_path
   if file_pate:
      text_var.set(file_path) # 标签显示文件名

# 创建主窗口
root = tk.Tk()
root.title("File Selection GUI")

# 创建按钮，点击按钮调用 open_file_dialog 函数
button = tk.Button(root, text="选择文件", command=open_file_dialog)
button.pack(pady=10)

# 创建文本显示窗口
text_var = tk.StringVar() # 创建一个StringVar 变量类型，用于实现实现动态更新，open_file_dialog()函数中就是操作这个变量。
text_label = tk.Label(root, textvariable=text_var, wraplength=400)
text_label.pack(pady=10)

# 启动主循环
root.mainloop()

```

# 运行效果

![avatar](/images/gui-select-show.png)
