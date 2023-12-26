---
title: 在图片的不同区域增加不同的超链接
date: 2023-10-31 15:23:46
categories:
- Python学习与实践
- 学习总结
---

# 代码

```html
<html>
<head>
    <!-- 设置页面标题 -->
    <title>点击图片的左边是百度，右边是微博</title>
</head>

<body>
    <!-- 插入图片，并应用图像映射 -->
    <img src="./icon-hexo.png" usemap="#top_bg"/>

    <!-- 定义图像映射 -->
    <map name="top_bg">
        <!-- 定义百度链接的矩形区域 -->
        <area alt="百度" href="http://www.baidu.com" shape="rect" target="blank" coords="0,0,300,300"/>
        
        <!-- 定义微博链接的矩形区域 -->
        <area alt="微博" href="http://weibo.com" shape="rect" target="blank" coords="400,0,700,400"/>
    </map>
</body>
</html>

```

# 效果

点击图片左右侧将分别跳转不同链接。

<img src="https://picsum.photos/700/300" usemap="#top_bg"/>

<map name="top_bg">
    <area alt="百度" href="http://www.baidu.com" shape="rect" target="blank" coords="0,0,300,300"/>
    <area alt="微博" href="http://weibo.com" shape="rect" target="blank" coords="400,0,700,400"/>
</map>
