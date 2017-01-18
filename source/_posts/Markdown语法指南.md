---

title: Markdown语法指南

date: 2016-06-05 22:41:49

tags: Markdown

---

简单记录下Markdown基础语法。

## 标题

	# 一级标题
	## 二级标题
	### 三级标题
	#### 四级标题
	##### 五级标题
	###### 六级标题

<!--more-->

## 列表

无序列表：(星号会被圆点替代)

	* Mac OSX
	* Windows
	* Linux
	* Unix

有序列表：(效果一样)

	1. Mac OSX
	2. Windows
	3. Linux
	4. Unix

## 引用

	> 这是一段引用文字。

> 这是一段引用文字。

## 插入链接

	[百度一下](http://www.baidu.com)，你就知道。

[百度一下](http://www.baidu.com)，你就知道。

## 插入图片

	![风景](http://img2.imgtn.bdimg.com/it/u=397276370,1341734514&fm=21&gp=0.jpg)

![风景](http://img2.imgtn.bdimg.com/it/u=397276370,1341734514&fm=21&gp=0.jpg)

## 斜体和粗体

	我是*斜体字*，我是**粗体字**，我是***斜体字加粗***。

我是*斜体字*，我是**粗体字**，我是***斜体字加粗***。

## 分割线

	***或---

---

## 代码块

### 行内代码块

	iOS中使用`NSLog(@"Hello World")`输出日志。

iOS中使用`NSLog(@"Hello World")`输出日志。

### 段代码块

代码块前后各3个"`"。（为了解决显示问题，下面语法中的某些符号用单引号"'"代替）

    ``'
    代码块...
    ``'

```
// js to oc
JSContext *context = [[JSContext alloc] init];
[context evaluateScript:@"var num = 5 + 5"];
[context evaluateScript:@"var names = ['Lucy', 'Lance', 'Lily']"];
[context evaluateScript:@"var triple = function(value) {return value * 3}"];
JSValue *tripleNum = [context evaluateScript:@"triple(num)"];
NSLog(@"triple num = %lf", tripleNum.toDouble);
```

### 文本段块

每行前面加四个空格或者一个tab。类似于段代码块，但是在每行前面不会有行数。

	PHP是世界上最好的语言；
	Java是世界上最好的语言。
	Objective-C是世界上最好的语言;

## 表格

A simple table looks like this:

	First Header | Second Header | Third Header
	------------ | ------------- | ------------
	Content Cell | Content Cell  | Content Cell
	Content Cell | Content Cell  | Content Cell

If you wish, you can add a leading and tailing pipe to each line of the table:

	| First Header | Second Header | Third Header |
	| ------------ | ------------- | ------------ |
	| Content Cell | Content Cell  | Content Cell |
	| Content Cell | Content Cell  | Content Cell |

Specify alignement for each column by adding colons to separator lines:

	First Header | Second Header | Third Header
	:----------- | :-----------: | -----------:
	Left         | Center        | Right
	Left         | Center        | Right

效果如下：

First Header | Second Header | Third Header
:----------- | :-----------: | -----------:
Left         | Center        | Right
Left         | Center        | Right
