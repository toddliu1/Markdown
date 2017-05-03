# <p align="middle">MarkDown基本语法</p>


**My Profile**  

- Name:Todd Liu  
- QQ:190359014  
- Email:twl2041@126.com  


## 1. 标题

syntax：用1到6个前导“#”表示六级标题  

demo:

\# **<font size=6>标题1</font>**  
\## **<font size=5>标题2</font>**  
\### **<font size=4>标题3</font>**  
**·**  
**.**  
\###### **<font size=2>标题6</font>**  


## 2. 段落

syntax：段落结束跟两个“空格”表示段落，换行  

demo:  

Hello MarkDown.  
My name is Todd Liu.  
There are **TWO Spaces** follow every paragraph.  


## 3. 强调

syntax：用2个星号“*”表示加粗；1个星号表示斜体；3个星号加粗倾斜  

demo:  

\*\*Demo\*\*  **粗体**  
\*Demo\*  *斜体*  
\*\*\*Demo\*\*\*  ***加粗倾斜***  
~~Demo删除线~~  


## 4. 列表

### 4.1 无序列表

syntax："*"或者"-"或者"+" 加一个空格，和前面段落要有空行  

demo:  

\- Name：Todd Liu  
\- Email：twl2041@126.com   
\- Address：Xi'an , Shaanxi , China  

显示效果：

- Name：Todd Liu  
- Email：twl2041@126.com
- Address：Xi'an , Shaanxi , China  

### 4.2 有序列表

syntax：数字+点+空格，不按数字排序也可以，markdown会自动重排   

demo:  

1. Name：Todd Liu
2. Address：Xi'an , Shaanxi , China
3. Email：twl2041@126.com
5. QQ：190359014
4. Phone：13891769612


## 5. 链接

syntax：\[链接文字](URL)

### 5.1 内嵌式链接

- 外部链接

	syntax：\[链接文字\]（网址）  

	demo： [百度](http://www.baidu.com)  

- 内部链接

	- 方式1：链接到仓库的其他文件  \[链接文字](文件名)

	- 方式2：链接到本文档其他部分，类似书签  \[链接文字] (文件名#标题)

	注：如果标题中有空格可以用“ - ”代替  

### 5.2 引用式链接

方式：在文档最末尾链接区定义链接，在文中引用。链接区定义链接的代码实际不会显示。  
好处：大量相同引用可以简化；便于修改，只需修改链接区即可。  

syntax：引用链接 [链接文字]，在文末链接区用 [链接文字]：URL 来定义链接  

demo：  

51cto网站链接 [51cto]  
demo文件的链接 [demo]  
本文档的链接 [标题]  
定义别名：[百度][baidu]  


## 6. 图片

syntax：![alt](URL “text”)  
alt是图片无法正常显示时展示的文字；URL是图片的链接；text是鼠标放到图片上显示的文字  

### 6.1 内嵌式图片

- 外部图片  

	demo：

	![baidu_logo](https://www.baidu.com/img/bd_logo1.png “百度一下”)  

- 仓库内部图片

	syntax：仓库中图片的相对路径  

	demo：

	\!\[img_erro]\(images/logo1.png)   

	![img_erro](images/logo1.png)


### 6.2 引用式图片

syntax：用 ![图片链接文字] 引用，在链接区定义图片链接 [图片链接文字]:图片路径  

demo：

\!\[md_logo]  

![md_logo]


## 7. 引用

syntax：引用的文字前面加“>”，多重引用加多个大于号，如“>>” ， “>>>”  

demo:

>这是第一则引文。  
>这是第二则引文。  
>这是第三章引文。  

多重引文：  

>第1重引文。  
>>第2重引文。  
>>>第3重引文。  


## 8. 代码块

- 行内代码

	syntax：使用一对反引号引起来表示行内的代码

	demo:

	其中第一行`#!/bin/bash`表示bash解释器路径
  
- 代码块  

	syntax：使用前导两个Tab或者八个以上空格表示代码块  
	
	demo:


		#! /bin/bash

		echo "hello world"
		exit 0


## 9. 表格

syntax：第一行用“ | ”隔开表示表头，第二行用“ | ”和“ - ”表示分割线，其余表的每列用“|”分隔  

demo:  

表头    |name|id|address|phone|  
分割线  |----|----|----|----|  
表的行  |Todd|01|shaanxi|12345|  
表的行  |Tom|02|london|22333|  
表的行  |Anna|03|newyork|38933|  

显示效果：

|name|id|address|phone|
|----|----|----|----|
|Todd|01|shaanxi|12345|
|Tom|02|london|22333|
|Anna|03|newyork|38933|


## 10. 注释

注释的方法有两种：

- 行注释  
syntax：[^_^]:本行是注释  

- 块注释  
syntax：\<!-- 下面是本文中的链接 -->  


## 11. 兼容HTML语法

注意：MarkDown语法完美兼容html语法，但不可以在html代码内使用markdown  


### 11.1 设置字体

syntax：\<font size=# face="字体" color=“颜色”>需要设置字体的文字\</font>

demo：

这一行是原始大小的字体  

<font size=6 face="微软雅黑" color="red">这一行是微软雅黑6磅红色文字</font>  

其他html样式：  

demo：

\<b>表示加粗样式：<b>这是一行加粗的文字</b>  
\<i>表示倾斜样式：<i>这是一行倾斜的文字</i>  
\<s>表示删除线样式：<s>这是一行删除线</s>  
\<u>表示下划线样式：<u>这一行加了下划线</u>  
\<sup>表示上标：A<sup>x</sup>  
\<sub>表示下标：B<sub>y</sub>  

### 11.2 设置图片大小
syntax：\<img src="path_to_picture" width="#" height="#">\</img>

demo：

![md_logo]
<img src="images/md_logo.png" width="64" height="64"></img>

### 11.3 表格

syntax：

\<table>\</table>表示表格范围  
\<tr>\</tr>表示表格的一行  
\<th>\</th>表示标题行  
\<td>\</td>表示数据行  


demo：

<table>
<tr>
	<th>姓名</th>
	<th>ID</th>
	<th>家庭地址</th>
	<th>电话号码</th>
</tr>

<tr>
	<td>tom</td>
	<td>11111</td>
	<td>陕西西安</td>
	<td>18282882</td>
</tr>

<tr>
	<td>jack</td>
	<td>22222</td>
	<td>北京市</td>
	<td>87848484</td>
</tr>

</table>

### 11.4 段落标记

- 使用**\<p />表示段落段落**

- 使用**\<br />表示单行**  
demo： 插入空行用\<br />




<!-- 下面是本文中的链接 -->

[51cto]:http://www.51cto.com  
[demo]:demo.md  
[标题]:MarkDown.md#标题  
[baidu]:http://www.baidu.com  
[md_logo]:images/md_logo.png


# END  ……
