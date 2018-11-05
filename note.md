超文本标记语言	HTML

认识Style元素
<style type="text/css">
	body {
		background-color : #d2b48c;			//设置背景颜色
		margin-left : 20%;					//设置左边距占页面的20%
		margin-right : 20%;					//设置右边距占页面的20%
		border : 2px dotted black;			//定义页面主题周围的边框虚线，颜色为黑色
		padding : 10px 10px 10px 10px;		//在body里面创建内边距
		font-family : sans-serif;			//定义文本使用的字体
	}
</style>

1920 * 1080

CSS 是层叠样式 (Cascading Style Sheets)的缩写，用来控制HTML的表现

所有html 的页面都要有一个<html>元素，其中要有一个<head>元素和一个<body>元素

网页的信息放在<head>元素里

<body>元素里的内容就是你将在浏览器里看到的东西，大多数空白符(制表符、回车、空格)都会被浏览器忽略，可以利用空白符让你的HTML
更有可读性。

可以在<style>元素中写CSS规则，为HTML网页增加CSS。<style>元素总要放在<head>元素里

可以使用CSS在HTML中指定元素的特性

http://wickedlysmart.com/hfhtmlcss

了解属性
	利用属性,可以指定一个元素的附加信息。 type属性指定我们使用哪一种样式语言，这里就是CSS
	
href 的含义是 hypertextreference "超文本引用"


<a href="cv.html">Resume</a>
Eye Candy
<a href="mini-cooper.html">See my mini</a>
millionaire.html

链接资源的相对路径
(1)向下链接到一个子文件夹

(2)向上链接到一个"父文件夹"
cd ..	到父文件夹
.. 表示父文件夹

三、创建网页，构建模块
	标记、元素、链接、路径......, 从概念到蓝图来设计web页面，会增加一些新工具

标记引用
<q></q>

<blockquote> 元素用语比较长的引用，需要单独显示
<blockquote> 创建了单独的一个文本块(与<p>类似),另外还把文字稍稍缩进，使它更像
一个引用

<q>和<blockquote>实际是两类不同的元素。<blockquote>元素是一个块(block)元素,而<q>元素是一个内联(inline)元素。
块元素显示时前后各有一个换行，而内联元素在页面文件流中总在"行内"出现。

块元素: 特立独行
<h1>、<h2>、....、<h6>、<p>和<blockquote>
每个块元素都单独显示，好像前后都有换行,块元素内容分块显示

内联元素: 随波逐流
<q>、<a>和<em>是内联元素
内联元素会显示在所在的段落中

块元素和内联元素:	块元素通常用作Web页面中的主要构建模块，而内联元素往往用来标记小段内容。设计
页面时，一般先从较大的块开始(块元素)，然后在完善页面时再加入内联元素。在用CSS控制HTML的表现时，这些知识就能派上用场了。

把一个元素放在另一个元素中称为"嵌套"


<br>	元素是一个没有任何内容的元素。它只是一个换行，没有其他内容。<br>并不是唯一没有实际内容的元素，还有很多类似这样的元素，我们把这些
元素叫做void元素。比如<img>元素。

P141

我是一级标题					<h1>			块元素
我时刻准备链接到另一个页面		<a>				内联元素		(a元素可以包围块元素,而不只是文本，所以，根据具体的上下文,<a>既可以是内联元素也可以是块元素)
用我强调文本					<em>			内联元素
我是个列表，不过我不关心
顺序							<ul>			块元素
我是正真的换行符				<br>			
我是放在列表中的列表项			<li>			块元素
我要保证我的列表有序			<ol>			块元素
我的任务就是提供图像			<img>			内联元素
用我可以在段落中加引用			<quote>			内联元素
用我来引用独立的文字			<blockquote>	块元素

对应特殊字符的字符实体
&amp;		html中显示	

链接起来

统一资源定位符	(Uniform Resource Locator,	URL)是一个全局地址，可以用来定位web上的任意资源，
包括html页面，音频、视频和其他形式的web内容


A		http://www.earlsautos.com
B		http://www.earlsautos.com/directions.html
C		http://www.earlsautos.com/cars/new/
D		http://www.earlsautos.com/cars/used/inventory.html
E		http://www.earlsautos.com/cars/new/images/minicooper.gif

使用id属性为<a>创建目标
	带id的元素有一个特殊特性: 你可以直接链接这些元素。
	使用id属性在页面中为<a>创建目标???
	(1)找到页面中你希望创建锚点的位置。可以是也页面上的任何文本，通常是标题
	(2)为目标选择一个标识符名，并在元素的开始标记中插入一个id属性。
	
如果一个匀元素里有两个属性，属性的先后顺序重要吗？例如，title属性是不是总在href后面?
	所有元素中，属性的顺序都不重要，可以使用任何顺序
	
	
链接到一个新窗口
	使用target打开新窗口，要在一个新窗口中打开一个页面，需要告诉浏览器你要打开的窗口名。如果没有告诉浏览器
要使用哪个特定的窗口，浏览器就会在同一个窗口中打开这个页面。可以为<a>元素增加一个target属性，告诉浏览器会在
同一个窗口中打开这个页面。如果使用"_blank"作为目标，浏览器就总是打开一个新窗口显示页面。
