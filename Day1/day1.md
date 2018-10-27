# HTML基础 #

----------

## HTML标题 ##
	html标题（heading）是通过<h1>-<h6>标签定义的
```
<h4>这是一个标题h4<h1>
<h5>这是一个标题h5<h2>
<h6>这是一个标题h6<h3>
```
## HTML段落 ##
```
<P>这是一个段落</p>
<P>这是另外一个段落</p>
```
## HTML链接 ##
```
<a href="http://www.runoob.com">这是 一个链接</a>
```
## HTML图像 ##
```
<img src="/images/logo.png" width="258" height="39" />
```
注意：图像的名称和尺寸是以属性形式提供的

## 笔记 ##
	1、*.html 文件跟 *.jpg 文件(f盘)在不同目录下：
	<img src="file:///f:/*.jpg" width="300" height="120"/>
	2、*.html 文件跟 *.jpg 图片在相同目录下：
	<img src="*.jpg" width="300" height="120"/>
	3、*.html 文件跟 *.jpg 图片在不同目录下： 
	a、图片 *.jpg 在 image 文件夹中，*.html 跟 image 在同一目录下：
	<img src="image/*.jpg/"width="300" height="120"/>
	b、图片 *.jpg 在 image 文件夹中，*.html 在 connage 文件夹中，image 跟 connage 在同一目录下：
	<img src="../image/*.jpg/"width="300" height="120"/>
	4、如果图片来源于网络，那么写绝对路径：
	<img src="http://static.runoob.com/images/runoob-logo.png" width="300" height="120"/>

	**HTML 中 href、src 区别**
	href 是 Hypertext Reference 的缩写，表示超文本引用。用来建立当前元素和文档之间的链接。常用的有：link、a。
	例如：
	<link href="reset.css" rel=”stylesheet“/>
	浏览器会识别该文档为 css 文档，并行下载该文档，并且不会停止对当前文档的处理。这也是建议使用 link，
	而不采用 @import 加载 css 的原因。 src 是 source 的缩写，src 的内容是页面必不可少的一部分，是引入。
	src 指向的内容会嵌入到文档中当前标签所在的位置。常用的有：img、script、iframe。
	例如:
	<script src="script.js"></script>
	当浏览器解析到该元素时，会暂停浏览器的渲染，直到该资源加载完毕。这也是将js脚本放在底部而不是头部得原因。
	简而言之，src 用于替换当前元素；href 用于在当前文档和引用资源之间建立联系。

# HTML元素 #
**HTML文档由HTML元素定义。**

开始标签|元素内容|结束标签
:--:|:--:|:--:
&lt;p>|这是一个段落|&lt;/p>
&lt;a href="default.htm">|这是一个链接|&lt;/a>
&lt;br>|换行|none
	开始标签常被称为起始标签（opening tag），结束标签常称为闭合标签（closing tag）
## HTML语法 ##
- HTML元素以开始标签起始
- HTML元素以结束标签终止
- 元素的内容是开始标签与结束标签之间的内容
- 某些HTML元素具有空内容（empty content）
- 空元素在开始标签中进行关闭（以开始标签的结束而结束）
- 大都数HTML元素可拥有属性

## 嵌套的HTML元素 ##
HTML文档由嵌套的HTML元素组成。
### HTML文档实例 ###
```
<DOCTYPE html>
<html>

<body>
<p>这是一个段落。</p>
</body>

</html>
```
## 笔记 ##
	1. 一些标签的使用，切记所有标签都需要闭合，不管是单体标签还是成对标签。（尽管目前浏览器是
		识别有些标签不闭合的情况，但是取的最好的保证兼容性，使用闭合）
	2. 标签写法要用小写字母（有些版本对大小写可认为相同，而xhtml中强制使用小写）

# HTML属性 #
**属性是HTML元素的附加信息**
### HTML属性 ###
- HTML元素可以设置属性
- 属性可以在元素中添加附加信息
- 属性一般描述于开始标签
- 属性总是以名称／值队的形式出现，比如：name="value"

	HTML 属性常用引用属性值
	属性值应该始终被包括在引号内。
	双引号是最常用的，不过使用单引号也没有问题。
	提示: 在某些个别的情况下，比如属性值本身就含有双引号，那么您必须使用单引号，例如：name='John "ShotGun" Nelson'

### HTML属性参考手册 ###
查看完整的HTML属性列表:<a href="http://www.runoob.com/tags/html-reference.html">HTML属性参考手册</a>
下面列出了适用于大多数HTML元素的属性:

属性|描述
:--:|:--:
class|为html元素定义一个或多个类名(classname)(类名从样式文件引入）
id|定义元素唯一id
style|规定元素的行内样式（inline style）
title|描述了元素的额外信息 (作为工具条使用)

更多标准属性说明：<a href="http://www.runoob.com/tags/ref-standardattributes.html">HTML标准属性参考手册</a>

## 笔记 ##
	属性和属性值，尽量小写，本来这样做也方便些。
	class 属性可以多用 class=" " （引号里面可以填入多个class属性）
	id 属性只能单独设置 id=" "（只能填写一个，多个无效）

10/27/2018 11:37:23 PM 