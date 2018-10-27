# HTML基础 #

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
	href 是 Hypertext Reference 的缩写，表示超文本引用。用来建立当前元素和文档之间的链接。常用的有：link、a。例如：
	<link href="reset.css" rel=”stylesheet“/>
	浏览器会识别该文档为 css 文档，并行下载该文档，并且不会停止对当前文档的处理。这也是建议使用 link，而不采用 @import 加载 css 的原因。 src 是 source 的缩写，src 的内容是页面必不可少的一部分，是引入。src 指向的内容会嵌入到文档中当前标签所在的位置。常用的有：img、script、iframe。例如:
	<script src="script.js"></script>
	当浏览器解析到该元素时，会暂停浏览器的渲染，直到该资源加载完毕。这也是将js脚本放在底部而不是头部得原因。
	简而言之，src 用于替换当前元素；href 用于在当前文档和引用资源之间建立联系。