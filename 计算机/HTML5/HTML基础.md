# HTML基础

HTML基本框架：标签、属性、元素

HTML不区分大小写

标签
  分成对称标签和非对称标签
		对称标签：如<p 属性>…</p>等，以<标签名 属性>…</标签名>形式出现，形成闭环，其中/用来表示结束

		非对称标签：如<br 属性/>，以<标签名 属性/>出现，/依旧表示结束


<!DOCTYPE>：声明HTML文档采用什么类型的编写指令
<html></html>：最大的元素，表示整个文档
<title></title>：嵌套在head中，显示标题
<body></body>：表示文档的正文部分，即设置浏览器显示的正文
<!--  -->：注释




Html元信息：
<head>
<meta>
<base>




## 表单

form
input
textarea
label
fieldset：定义域
legend：定义域的标题
<select></select>：下拉选单
  <option>...</option>：选项
<optgroup></optgroup>：将标签进行组合（没多大意义）
<button></button>


HTML5：

datalist
keygen
output


## 列表

<ol></ol>：有序列表框架，列表项前面用数字表示
<ul></ul>：无序列表框架
<li></li>：嵌套在列表框架（ul\ol等）中，表示列表的一项，默认会在每一项前面加上小实心圆

<dl></dl>：自定义列表框架，中间嵌套具体内容
<dt></dt>：表示自定义列表每一项的标题
<dd></dd>：表示自定义列表每一项的内容



## 块排版

<div></div>
<span></span>





框架
<frame>
<frameset>
<noframes>
<iframe>



HTML5：
<header>：定义页面或小节的页眉
<footer>：定义页面或小节页脚
<section>：定义小节

<article>
<aside>



## 表格

<table></table>：生成一个小框架
  border=""：边界线的宽度，0表示没边界线
	cellpadding=""：表示cell（即填充文字等的地方）与表格框的距离
	cellspacing=""：表示表格框之间的距离
<caption></caption>：表格标题
<tr></tr>：表示一行，中间嵌套<th>或<td>
<th></th>：表示列表表头的单元格，相当于数据库表的属性，默认加粗
<td></td>：表示列表记录的单元格，相当于数据库表的记录

<thead></thead>：定义表格的页眉，和下面两个一样用于将表格分块，相当于易于交互的过程
<tbody></tbody>：定义表格的页身
<tfoot></tfoot>：定义标的页脚

<col />：用来定义每列的对齐方式
<colgroup></colgroup>：分组进行对齐设置



## 文本
段落：
  <p></p>：段标签
	<br />：换行

标题：
	<h1></h1>~<h6></h6>：显示标题，h1是文档的总标题，一个文档只能有一个，其它则没有限制


文本格式：
	<hr>：定义水平线

	<b></b>：粗体
	<i></i>：斜体
	<big></big>：大号字体
	<small></small>：小号字体

	<em></em>：强调文字
	<strong></strong>：更加强调文字

	<sub></sub>：定义下标
	<sup></sup>：定义上标
	<ins></ins>：下划线
	<del></del>：删除线


计算机输出标签
<code>
<samp>
<kbd>
<tt></tt>
<var>
<pre>


引用、术语定义
<dfn>
<cite>


<acronym>
<abbr>
<address>



## 链接

<a></a>：超链接
  href="#id号码"：用来跳转到id号码对应的位置
	href="网址"：跳转到网址
	href="mailto:邮箱地址"：创建邮箱协议超链接，用来发送邮件内容

<link></link>：链接外部样式表
	href：指明样式表文件的位置
  rel：规定当前文档与被链接文档之间的关系，默认只有stylesheet属性得到所有支持
  media：规定显示的设备类型
  type：规定文档MIME类型，现在只有text/css属性，几乎可省略

<nav>：导航链接


## 外部编程

<script></script>：定义客户端脚本
<noscript>：当不支持客户端脚本时候的替代内容
<embed>：为外部程序定义框架

<style>：定义外部CSS

<object>
<param>


## 多媒体

图像
  <img />：引用图像
		src=""：表示图像的位置
		alt=""：当图象因为某种原因无法显示时候的代替文字
		title=""：鼠标悬停在图片上的说明文字
		height=""：图片高度
		width=""：图片宽度
	<map>：定义图像内部映射
	<area>：

	HTML5：
	<canvas>：图像容器
	<figcaption>：图像标题
	<figure>：规定独立的流媒体


音/视频（HTML5）：
	audio：定义音频
	video：定义视频
	source：定义多份资源，由浏览器选择支持类型


## 公共属性

id
class
style
title


## 符号
&lt;：小于号
&gt;：大于号
&quot;：双引号
&amp;：&运算符
&nbsp;：空格







# HTML5语义化标签

article
section
aside
hgroup
header
footer
nav
time
mark
figure
figcaption





<bdi></bdi>
<bdo></bdo>




<table>
  <thead>
    <tr>
      <th>名字</th>
      <th>学号</th>
    </tr>
  </thead>

  <tbody>
    <tr>
      <th>A</th>
      <th>12</th>
    </tr>
    <tr>
      <th>B</th>
      <th>13</th>
    </tr>
  </tbody>

  <tfoot>
    <tr>
      <th>一起</th>
      <th>一起</th>
    </tr>
  </tfoot>
</table>




两大隐藏显示利器
target
checkout



几个问题：

1、苹果公司成功的原因
2、mac不成功而iphone成功的原因
3、google为什么还要出chromebook
