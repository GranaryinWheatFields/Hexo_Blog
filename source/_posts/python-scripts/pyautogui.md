---
title: pyautogui
date: 2023-10-31 15:23:46
categories:
- Python学习与实践
- 学习总结
---

# 简介

pyautogui 是一个用于自动化鼠标和键盘操作的 Python 库。它可以用于创建自动化脚本，执行重复性任务，模拟用户输入等。

# 函数及其说明

| 功能分类           | 功能描述和示例                                           |
|--------------------|----------------------------------------------------------|
| **鼠标操作**        |                                                          |
| 获取鼠标位置       | `x, y = pyautogui.position()`                              |
| 移动鼠标到指定位置   | `pyautogui.moveTo(x, y, duration=1)`                       |
| 移动鼠标相对距离     | `pyautogui.move(100, 50, duration=1)`                     |
| 点击鼠标左键         | `pyautogui.click(x, y)`                                   |
| 点击鼠标右键         | `pyautogui.rightClick(x, y)`                              |
| 点击鼠标中键         | `pyautogui.middleClick(x, y)`                             |
| 拖拽鼠标             | `pyautogui.dragTo(x, y, duration=1)`                      |
| **键盘操作**        |                                                          |
| 发送按键             | `pyautogui.press('enter')`                                |
| 发送组合键           | `pyautogui.hotkey('ctrl', 'c')`                           |
| 输入文本             | `pyautogui.typewrite('Hello, World!')`                   |
| **屏幕截图**        |                                                          |
| 截取整个屏幕         | `screenshot = pyautogui.screenshot()`                     |
| 截取指定区域         | `screenshot = pyautogui.screenshot(region=(x, y, w, h))` |
| **延迟和速度控制**   |                                                          |
| 设置全局暂停时间     | `pyautogui.PAUSE = 1`                                     |
| 控制动作速度         | `pyautogui.moveTo(x, y, duration=2)`                      |
| **异常处理**        |                                                          |
| 添加异常处理         | ```python try: pyautogui.click(x, y) except Exception as e: print(f"Error: {e}") ``` |
| **其他功能**        |                                                          |
| 获取屏幕分辨率       | `width, height = pyautogui.size()`                         |
| 获取像素颜色         | `color = pyautogui.pixel(x, y)`                           |
| 滚动鼠标滚轮         | `pyautogui.scroll(10)`                                    |
