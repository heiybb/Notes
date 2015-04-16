DOM是针对HTML和XML的API，但是它独立于任何编程语言和环境，即你可以用java、javaScript和其它语言来使用它，但是由于javascript的特殊性——主要负责HTML的显示，所以DOM默认为JavaScript的三大标准组件之一


这里主要介绍1998年W3C的推荐标准DOM1


DOM1被完全支持的浏览器：

DOM1规定了节点层次和一个Node接口，其中接口用来实现所有的节点类型，而这个接口在实现时是以Node类型（就把它想象成一个类吧）来实现的，大部分浏览器（除了IE）都可以访问这个类型。

而其它所有的类型都继承自这个Node类型，以下为节点的公共属性和方法：
  nodeName：
	nodeValue：
	nodeType：表明当前节点的属性类型，DOM1定义有以下12种类型
		Node.ELEMENT_NODE(对应nodeType值为1)
		Node.ATTRIBUTE_NODE(2)
		Node.TEXT_NODE(3)
		Node.CDATA_SECTION_NODE(4)
		Node.ENTITY_PEFERENCE_NODE(5)
		Node.ENTITY_NODE(6)
		Node.PROCESSING_INSTRUCTION_NODE(7)
		Node.COMMENT_NODE(8)
		Node.DOCUMENT_NODE(9)
		Node.DOCUMENT_TYPE_NODE(10)
		Node.DOCUMENT_FRAGMENT_NODE(11)
		Node.NOTATION_NODE(12)



节点关系：
操作节点：





Document类型：即当前作用页面的实例化文本，它的任何方法都是针对当前页面进行的，以下为属性和方法列表
	URL：当前页面的完整url地址
	domain：当前页面的域名
	title：当前文档的标题
	childNodes：子节点
	firstChild：
	body：当前文档的body部分
	doctype：取得<!DOCTYPE>的引用
	
	anchors：返回所有带name特性的<a>元素
	applets：返回所有<applet>元素
	forms：返回所有带<form>元素
	images：返回所有<img>元素
	links：所有带href特性的<a>元素
	
	implementation：检查浏览器是否支持什么功能
	
	getElementById()：通过id来查找元素
		IE8及低版本不区分ID大小写
	getElementsByTagName()：通过元素的标签名来查找元素
	
Element类型：用于表现XML和HTML元素的
Text类型：
Comment类型：
CDATASection类型：
DocumentType类型：
DocumentFragment类型：
Attr类型：