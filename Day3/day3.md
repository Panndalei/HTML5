# HTML表格 #
```
<table border="1">
    <tr style="background-color:green">
        <th>row 1, cell 1</th>
        <th>row 1, cell 2</th>
    </tr>
    <tr>
        <td>row 2, cell 1</td>
        <td>row 2, cell 2</td>
    </tr>
</table>
```
## HTML表格表头 ##
表格的表头使用 &lt;th> 标签进行定义。大多数浏览器会把表头显示为<th>粗体居中的文本.</th>

## HTML列表 ##
### 无序列表 ###
无序列表是一个项目的列表，此列项目使用粗体圆点（典型的小黑圆圈）进行标记。
无序列表使用 &lt;ul> 标签
```
<ul>
<li>Coffee</li>
<li>Milk</li>
</ul>
```
<ul>
<li>Coffee</li>
<li>Milk</li>
</ul>

### 有序列表 ###
有序列表也是一列项目，列表项目使用数字进行标记。 有序列表始于 &lt;ol> 标签。每个列表项始于 <li> 标签。
列表项使用数字来标记。
```
<ul>
<li>Coffee</li>
<li>Milk</li>
</ol>
```
<ol>
<li>Coffee</li>
<li>Milk</li>
</ol>

### 自定义列表 ###
自定义列表不仅仅是一列项目，而是项目及其注释的组合。
自定义列表以 &lt;dl> 标签开始。每个自定义列表项以 &lt;dt> 开始。每个自定义列表项的定义以 &lt;dd> 开始。
```
<dl>
<dt>Coffee</dt>
<dd>- black hot drink</dd>
<dt>Milk</dt>
<dd>- white cold drink</dd>
</dl>
```
<dl>
<dt>Coffee</dt>
<dd>- black hot drink</dd>
<dt>Milk</dt>
<dd>- white cold drink</dd>
</dl>

## HTML&lt;div>和&lt;span> ##
<h3>HTML 可以通过 &lt;div> 和 &lt;span>将元素组合起来。</h3>
### HTML区块元素 ###
大多数 HTML 元素被定义为块级元素或内联元素。
块级元素在浏览器显示时，通常会以新行来开始（和结束）。
实例: &lt;h1>, &lt;p>, &lt;ul>, &lt;table> 

### HTML内联元素 ###
内联元素在显示时通常不会以新行开始。
实例: &lt;b>, &lt;td>, &lt;a>, &lt;img>

### HTML &lt;div> 元素 ###

HTML &lt;div> 元素是块级元素，它可用于组合其他 HTML 元素的容器。
&lt;div> 元素没有特定的含义。除此之外，由于它属于块级元素，浏览器会在其前后显示折行。
如果与 CSS 一同使用，&lt;div> 元素可用于对大的内容块设置样式属性。
&lt;div> 元素的另一个常见的用途是文档布局。它取代了使用表格定义布局的老式方法。使用 &lt;table> 元素进行文档布局不是表格的正确用法。&lt;table> 元素的作用是显示表格化的数据。
### HTML &lt;span> 元素 ###
HTML &lt;span> 元素是内联元素，可用作文本的容器
&lt;span> 元素也没有特定的含义。
当与 CSS 一同使用时，&lt;span> 元素可用于为部分文本设置样式属性。

## HTML布局-使用&lt;div>元素 ##
```
<!DOCTYPE html>
<html>
<head> 
<meta charset="utf-8"> 
<title>HTML学习</title> 
</head>
<body>
 
<div id="container" style="width:500px">
 
<div id="header" style="background-color:#FFA500;">
<h1 style="margin-bottom:0;">主要的网页标题</h1></div>
 
<div id="menu" style="background-color:#FFD700;height:200px;width:100px;float:left;">
<b>菜单</b><br>
HTML<br>
CSS<br>
JavaScript</div>
 
<div id="content" style="background-color:#EEEEEE;height:200px;width:400px;float:left;">
内容在这里</div>
 
<div id="footer" style="background-color:#FFA500;clear:both;text-align:center;">
版权 © runoob.com</div>
 
</div>
 
</body>
</html>
```

<html>
<head> 
<meta charset="utf-8"> 
<title>菜鸟教程(runoob.com)</title> 
</head>
<body>
 
<div id="container" style="width:500px">
 
<div id="header" style="background-color:#FFA500;">
<h1 style="margin-bottom:0;">主要的网页标题</h1></div>
 
<div id="menu" style="background-color:#FFD700;height:200px;width:100px;float:left;">
<b>菜单</b><br>
HTML<br>
CSS<br>
JavaScript</div>
 
<div id="content" style="background-color:#EEEEEE;height:200px;width:400px;float:left;">
内容在这里</div>
 
<div id="footer" style="background-color:#FFA500;clear:both;text-align:center;">
版权 © runoob.com</div>
 
</div>
 
</body>
</html>
