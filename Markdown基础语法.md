



# Markdown基础教程

​                                                                                                                                                 ——嗜

*常用的应该就这么多吧，其它HTML元素、公式、流程图、时序图、甘特图等等应该用的不多吧。*

## 0.简介

Markdown 是一种轻量级标记语言，它允许人们使用易读易写的纯文本格式编写文档。

Markdown 语言在 2004 由约翰·格鲁伯（英语：John Gruber）创建。

Markdown 编写的文档可以导出 HTML 、Word、图像、PDF、Epub 等多种格式的文档。

Markdown 编写的文档后缀为 **.md**, **.markdown**。

*注意以下语法是在Typora软件下完成的*

## 1.标题

```
“# ”是一级标题（开头加# ）
```

````
“## ”是二级标题（开头加## ）
````

```
“### ”是三级标题（开头加### ）
```

+ **例如**

# 一级标题

## 二级标题

### 三级标题

---



## 2.字体

```
“* *”斜体（左右加**）
```

```
“** **”粗体（左右加** **）
```

```
“*** ***”粗斜体（左右加*** ***）
```

或

```
“_ _”斜体（左右加_ _）
```

```
“__ __”粗体（左右加__ __）
```

```
“___ ___”粗体（左右加___ ___）
```

+ 例如**

  *斜体*

  **黑体**

  ***斜黑体***
  
  
  
  _斜体_
  
  __黑体__
  
  ___斜黑体___
---



## 3.分割线

```
“---”分割线（三个---）细
“---”分割线（三个以上----）粗一点
```

或

```
“***”分割线（三个***）细
“***”分割线（三个以上****）粗一点
```



+ **例如**

___

____



***

****



## 4.删除线

```
“~~ ~~”删除线（前后加~~ ~~）
```

+ **例如**

  ~~删除线~~

---



## 5.下划线

```
<u>带下划线的文本</u>
```

+ **例如**

  <u>带下划线的文本</u>

---



## 6.脚注

```
句后要注释的角标[^1]
[^1]:这是角标的注释
```

+ **例如**

  句后要注释的角标[^1]

  [^1]:这是角标注释的内容

---



## 7.列表

列表支持有序列和无序列，简单来说就是前面是点的和前面是数字的。还会有一种列表里套列表，称作列表镶套。

**无序列表**

````
"* "第一项（前面带点的是句首加"* "）
或
"+ "第一项（前面带点的是句首加"+ "）
或
"- "第一项（前面带点的是句首加"- "）
````

+ **例如**
+ 星号带点

+ 加号带点

- 减号带点

**有序列表**

```
“1. ”第一项（数字加个点的是有序列表）
```

+ **例如**

1. 第一项
2. 第二项
3. 第三项

**嵌套列表**

```
“1. ”第1项
    “- ”第1.1项（注意这前面要有四个空格）
```

+ **例如**

1. 第1项
       - 第1.1项

---



## 8.区块

```
“>”区块引用
“>>”这样也可以嵌套使用
```

+ **例如**

> 区块引用

> 嵌套使用
>
> > 嵌套使用
> >
> > > 再嵌套

  **区块中也可以使用列表**

  ```
“>”区块中使用列表
“>1. ”带数字的第一项
“>2. ”带数字的第二项
“>+ ”带点的第一项
  ```

+ **例如**

> 区块中使用列表
>
> 1. 带数字的第一项
> 2. 带数字的第二项
>
> + 带点的第一项

  ​**列表中使用区块**

```
“* ”带点的第一项
    “>”列表中的引用1（注意这前面要有四个空格）
“1. ”带数字的第一项
    “>”列表中的引用1（注意这前面要有四个空格）
    “>>”列表中的区块嵌套使用（注意这前面要有四个空格）
```

+ **例如**

* 带点的第一项

  > 列表中的引用1

1. 带数字的第一项

   > 列表中的引用1
   >
   > >列表中的区块嵌套使用

---



## 9.代码的引用

**代码或者文字的加背景展示**

```
“`”print("hello world")“`”
“`”你好“`”
（需要展示单个代码片段，或者只是想展示以下加背景的文字，需要前后都加``）
```

+ **例如**

`print("hello world")`

`你好`

**代码区块的展示**

```
“```”python（这一行是输入什么语言，当然按回车也可以什么都不输入）
a="hello world"
print(a)
```

+ **例如**

```python
a="hello world"
print(a)
```

---



## 10.链接的使用

**文本带链接的使用法**

```
“[衔接的自定义的名称]”“（连接的地址）”   (注意这里的两个圆括号是英文输入法下的圆括号)
```

+ **例如**

[哔哩哔哩的链接](www.bilibili.com)

**直接链接地址**

```
“<www.bilibili.com>”
```

+ **例如**

<www.bilibili.com>

**在文字末尾附链接**（这功能感觉并没有设么用啊，难道我没学到精髓）

```
这个链接用1作为网址变量“[bilibili][1]”  （用1来代替链接）
这个链接用bilibili作为网址变量“[哔哩哔哩][bilibili]”  （用字母代替链接）
这个链接用币站作为网址变量“[哔哩哔哩][币站]

“[1]:www.bilibili.com”
“[bilibili]:www.bilibili.com”
“[币站]:www.bilibili.com”
```

+ **例如**

这个链接用1作为网址变量[bilibili][1] 
这个链接用bilibili作为网址变量[哔哩哔哩][bilibili]
这个链接用币站作为网址变量[哔哩哔哩][币站]



[1]:www.bilibili.com
[bilibili]:www.bilibili.com
[币站]:www.bilibili.com

---



## 11.图片的引用

**直接附一张图**

```
“![属性文本](地址)”     （注意都使用英文输入法）
或
“![属性文本](地址"赛博朋克")”     （注意都使用英文输入法） 当然显示效果貌似没啥区别
```

+ **例如**

![赛博朋克](http://i.17173cdn.com/2fhnvk/YWxqaGBf/cms3/crbfnrbnpzvbFFb.png)

![赛博朋克](http://i.17173cdn.com/2fhnvk/YWxqaGBf/cms3/crbfnrbnpzvbFFb.png"赛博朋克")

**在文字末尾附链接**（这功能感觉并没有设么用啊，难道我没学到精髓）

```
这个链接1作为网路变量“[赛博朋克][1]”

“[1]:www.xxx.xxx”
```

+ **例如**

这个链接1作为网路变量[赛博朋克][1]

[1]:http://i.17173cdn.com/2fhnvk/YWxqaGBf/cms3/crbfnrbnpzvbFFb.png

**另外还能指定图片的高度与宽度，可以使用<img>标签**

---



## 12.表格

```
“| | |”（使用这个符号就行，在Typora中直接输三个“|||”就会出表格，横向表格的多少是对应两竖中间的孔）

源代码模式下
“| | | |” (此为3格表)
“|:-|:-:|-:|”(从左到右依次为左对齐，居中，右对齐)
“| | | |”
(Typora软件不能通过代码调整往哪对齐-_-||)
```

+ **例如**

| 表格1 | 表格2 | 表格3 |
| :---: | :---: | ----: |
|       |       |       |



|表格4|表格5|表格6|
|:-|:-:|-:|
| 左对齐 | 居中 | 右对齐 |







***结尾分割线***

---



