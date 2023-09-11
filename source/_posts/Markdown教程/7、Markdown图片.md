---
title: 7、Markdown图片
date: 2023-09-07 17:00:00
categories: Markdown教程
tags: Markdown
---

# Markdown 图片语法
格式如下：
```
![alt 属性文本](图片地址)

![alt 属性文本](图片地址 "可选标题")
```
开头一个感叹号 !
接着一个方括号，里面放上图片的替代文字
接着一个普通括号，里面放上图片的网址，最后还可以用引号包住并加上选择性的 'title' 属性的文字。
使用实例：
```
![RUNOOB 图标](http://static.runoob.com/images/runoob-logo.png)

![RUNOOB 图标](http://static.runoob.com/images/runoob-logo.png "RUNOOB")
```

显示结果如下：
![RUNOOB 图标](http://static.runoob.com/images/runoob-logo.png)

![RUNOOB 图标](http://static.runoob.com/images/runoob-logo.png "RUNOOB")

# 使用变量
当然，你也可以像网址那样对图片网址使用变量:
```
这个链接用 1 作为网址变量 ![RUNOOB][RUNOOB-LOGO].
然后在文档的结尾为变量赋值（网址）

[RUNOOB-LOGO]: http://static.runoob.com/images/runoob-logo.png
```

显示结果如下：
这个链接用 1 作为网址变量 ![RUNOOB][RUNOOB-LOGO].
然后在文档的结尾为变量赋值（网址）

# 指定高度与宽度
Markdown 还没有办法指定图片的高度与宽度，如果你需要的话，你可以使用普通的 `<img>`标签。

```
<img decoding="async" src="http://static.runoob.com/images/runoob-logo.png" width="50%">
```
结果显示为：
<img decoding="async" src="http://static.runoob.com/images/runoob-logo.png" width="50%">
<img decoding="async" src="[1]" width="50%">

[RUNOOB-LOGO]: http://static.runoob.com/images/runoob-logo.png
