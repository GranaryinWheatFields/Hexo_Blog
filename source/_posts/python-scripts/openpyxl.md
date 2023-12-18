---
title: openpyxl
date: 2023-10-31 15:23:46
categories:
- Python学习与实践
- 学习总结
---

# 简介

`openpyxl` 是一个用于读写 Excel 文件（xlsx 格式）的 Python 库。它提供了丰富的功能，使你能够创建、修改和读取 Excel 文档。以下是关于 `openpyxl` 的详细介绍：


```bash
pip install openpyxl
```

## 基本用法

### 创建一个新的 Excel 文档：

```python
import openpyxl

# 创建一个新的 Excel 文档
workbook = openpyxl.Workbook()

# 获取默认的工作表
sheet = workbook.active

# 写入数据
sheet['A1'] = 'Hello'
sheet['B1'] = 'World'

# 保存文件
workbook.save('example.xlsx')
```

### 读取现有的 Excel 文档：

```python
import openpyxl

# 加载现有的 Excel 文档
workbook = openpyxl.load_workbook('example.xlsx')

# 获取默认的工作表
sheet = workbook.active

# 读取数据
value_A1 = sheet['A1'].value
value_B1 = sheet['B1'].value

print(f"A1: {value_A1}, B1: {value_B1}")
```

### 操作单元格：

```python
import openpyxl

# 创建一个新的 Excel 文档
workbook = openpyxl.Workbook()
sheet = workbook.active

# 写入数据
sheet['A1'] = 'Hello'
sheet['B1'] = 'World'

# 读取数据
value_A1 = sheet['A1'].value
value_B1 = sheet['B1'].value

print(f"A1: {value_A1}, B1: {value_B1}")

# 修改数据
sheet['A1'] = 'Updated Hello'

# 获取行和列
row_1 = sheet[1]
column_A = sheet['A']

# 迭代行或列
for cell in row_1:
    print(cell.value)

# 保存文件
workbook.save('example.xlsx')
```

### 操作表格：

```python
import openpyxl

# 创建一个新的 Excel 文档
workbook = openpyxl.Workbook()
sheet = workbook.active

# 添加表头
sheet.append(['Name', 'Age', 'City'])

# 添加数据
data = [('Alice', 25, 'New York'),
        ('Bob', 30, 'San Francisco'),
        ('Charlie', 22, 'Los Angeles')]

for row in data:
    sheet.append(row)

# 保存文件
workbook.save('table_example.xlsx')
```

## 高级功能

1. **样式设置：**

   `openpyxl` 允许设置单元格的样式，包括字体、颜色、对齐方式等。以下是一个简单的例子：

   ```python
   from openpyxl.styles import Font, Alignment

   # 创建一个新的 Excel 文档
   workbook = openpyxl.Workbook()
   sheet = workbook.active

   # 设置单元格样式
   cell = sheet['A1']
   cell.value = 'Styled Cell'
   cell.font = Font(bold=True, color='FF0000')  # 设置字体为粗体，颜色为红色
   cell.alignment = Alignment(horizontal='center', vertical='center')  # 设置水平和垂直对齐方式

   # 保存文件
   workbook.save('styled_example.xlsx')
   ```

2. **使用公式：**

   `openpyxl` 支持在单元格中使用公式。以下是一个使用公式的示例：

   ```python
   # 创建一个新的 Excel 文档
   workbook = openpyxl.Workbook()
   sheet = workbook.active

   # 添加数据
   sheet['A1'] = 10
   sheet['B1'] = 20

   # 在C1单元格中使用公式
   sheet['C1'] = '=SUM(A1:B1)'

   # 保存文件
   workbook.save('formula_example.xlsx')
   ```

3. **合并单元格：**

   `openpyxl` 允许合并单元格。以下是一个示例：

   ```python
   # 创建一个新的 Excel 文档
   workbook = openpyxl.Workbook()
   sheet = workbook.active

   # 合并单元格
   sheet.merge_cells('A1:D1')
   sheet['A1'] = 'Merged Cells'

   # 保存文件
   workbook.save('merged_cells_example.xlsx')
   ```

### `iter_rows()` 方法

`iter_rows()` 方法用于迭代指定范围内的行。以下是该方法的一般形式：

```python
iter_rows(min_row=1, max_row=None, min_col=1, max_col=None, values_only=False)
```

- `min_row`：迭代的起始行，默认为 1。
- `max_row`：迭代的结束行（不包括），默认为表格的最大行数。
- `min_col`：迭代的起始列，默认为 1。
- `max_col`：迭代的结束列（不包括），默认为表格的最大列数。
- `values_only`：如果为 `True`，则返回每行的单元格值而不是单元格对象。

示例：

```python
import openpyxl

workbook = openpyxl.load_workbook('example.xlsx')
sheet = workbook.active

# 迭代前两行的值
for row in sheet.iter_rows(min_row=1, max_row=2, values_only=True):
    print(row)
```

### `iter_cols()` 方法

`iter_cols()` 方法用于迭代指定范围内的列。以下是该方法的一般形式：

```python
iter_cols(min_col=1, max_col=None, min_row=1, max_row=None, values_only=False)
```

- `min_col`：迭代的起始列，默认为 1。
- `max_col`：迭代的结束列（不包括），默认为表格的最大列数。
- `min_row`：迭代的起始行，默认为 1。
- `max_row`：迭代的结束行（不包括），默认为表格的最大行数。
- `values_only`：如果为 `True`，则返回每列的单元格值而不是单元格对象。

示例：

```python
import openpyxl

workbook = openpyxl.load_workbook('example.xlsx')
sheet = workbook.active

# 迭代前两列的值
for col in sheet.iter_cols(min_col=1, max_col=2, values_only=True):
    print(col)
```

#### 注意事项：

- 如果 `values_only` 设置为 `True`，那么迭代结果将仅包含单元格的值，而不是单元格对象。
- 在迭代过程中，如果不指定 `min_row`、`max_row`、`min_col`、`max_col`，则将迭代整个工作表。
- 迭代的结果是一个生成器对象，你可以使用 `list()` 函数将其转换为列表，方便直接查看和处理数据。


# 函数及说明

以下是 `openpyxl` 中一些常用的函数和方法，使用表格的形式罗列并说明：

| 函数/方法                                        | 描述                                                         |
| ------------------------------------------------ | ------------------------------------------------------------ |
| **创建和保存文档**                                |                                                              |
| `openpyxl.Workbook()`                             | 创建一个新的 Excel 文档，返回一个工作簿对象。                |
| `workbook.save('filename.xlsx')`                 | 将工作簿保存为指定文件名的 Excel 文件。                     |
| `openpyxl.load_workbook('filename.xlsx')`        | 加载现有的 Excel 文件，返回一个工作簿对象。                  |
| **获取和操作工作表**                              |                                                              |
| `workbook.active`                                 | 获取默认的工作表对象。                                       |
| `workbook.create_sheet('SheetName')`             | 创建一个新的工作表，并返回工作表对象。                       |
| `workbook.sheetnames`                             | 获取所有工作表的名称列表。                                   |
| `workbook['SheetName']`                           | 获取指定名称的工作表对象。                                   |
| **读写单元格数据**                                |                                                              |
| `sheet['A1']`                                     | 获取指定单元格的单元格对象。                                 |
| `sheet['A1'].value`                               | 获取单元格的值。                                             |
| `sheet['A1'] = 'Data'`                            | 设置单元格的值。                                             |
| **迭代行和列**                                    |                                                              |
| `sheet.iter_rows(min_row=1, max_row=3, values_only=True)` | 迭代指定范围内的行，返回行的值。                             |
| `sheet.iter_cols(min_col=1, max_col=3, values_only=True)` | 迭代指定范围内的列，返回列的值。                             |
| **操作表格数据**                                  |                                                              |
| `sheet.append([data_row])`                        | 向工作表追加一行数据。                                       |
| `sheet.delete_rows(index, amount)`                | 删除指定索引和数量的行。                                     |
| `sheet.delete_cols(index, amount)`                | 删除指定索引和数量的列。                                     |
| **设置单元格样式**                                |                                                              |
| `cell.font = Font(bold=True, color='FF0000')`    | 设置单元格的字体样式，例如加粗和颜色。                       |
| `cell.alignment = Alignment(horizontal='center', vertical='center')` | 设置单元格的对齐方式，例如水平和垂直居中。                |
| **使用公式**                                      |                                                              |
| `sheet['C1'] = '=SUM(A1:B1)'`                     | 在单元格中使用公式。                                         |
| **合并和拆分单元格**                              |                                                              |
| `sheet.merge_cells('A1:D1')`                      | 合并指定范围内的单元格。                                     |
| `sheet.unmerge_cells('A1:D1')`                    | 拆分已合并的单元格。                                         |
| **设置列宽和行高**                                |                                                              |
| `sheet.column_dimensions['A'].width = 15`        | 设置指定列的宽度。                                           |
| `sheet.row_dimensions[1].height = 20`             | 设置指定行的高度。                                           |
| **图表和图形**                                  |                                                              |
| `openpyxl.chart.BarChart()`                       | 创建条形图对象。                                            |
| `chart.add_data(data, titles_from_data=True)`     | 向图表添加数据。                                            |
| `sheet.add_chart(chart, 'E5')`                   | 在指定位置插入图表。                                       |
| `openpyxl.drawing.image.Image('image_path.jpg')` | 创建图像对象。                                              |
| `sheet.add_image(image, 'C3')`                   | 在指定位置插入图像。                                       |
