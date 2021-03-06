# CSS基础

#### 基础结构
```
选择器{
    属性:值;
    属性:值;
    ...
｝
```




## 一、选择器

#### 派生选择器
```
后代选择器：
    需使用‘空格符’，a b表示元素a的所有b子元素（可相隔多层）都套用｛｝中的格式


子元素选择器：
	  需使用>（子结合符），a>b表示元素a的所有b儿子元素（即只能相隔一层）都套用｛｝中的格式

相邻兄弟选择器：
		需使用+（子结合符），a+b表示元素a后面和a同级的所有b元素都套用｛｝中的格式

	id选择器：以#接元素id（不加空格）

	类选择器：以.接元素class名称

	属性选择器：
		[a]：筛选出含属性名a的元素

	属性和值选择器：
		[a=b]：筛选出含属性值a且其值为b的元素
		[a~=b]：筛选出含属性a且其值中包含片段b的元素
		[a!=b]：筛选带有以指定值b开头的属性值的元素，b必须是整个单词
		[a^=b]：
		[a$=b]：
		[a*=b]：



## 二、样式表

#### 样式表的使用：
	外部样式表：通过元素<link>
	内部样式表（具有比外部样式表高的优先级——细化到单条属性）：通过元素<style>
	内联样式表：通过元素属性style


#### 样式表属性与值
```
	background-color：背景颜色属性
		默认值：transparent（透明）
		继承性：不继承
		可能的值：
			color_name（即直接的颜色名，red等）
			hex_name（十六进制的背景颜色，如#ff0000）
			rgb_number（用rgb函数表示，如rgb(255,0,0)）
			transparent（透明）
			inherit：规定可以从父辈继承颜色
	background-image：背景用图像填充
		默认值：none
		继承性：不继承
		可能的值：
			url('URL')：指明图像的路径
			none：即没有图像
			inherit：可继承
	background-repeat：规定背景图像的重复性
		默认值：repeat
		继承性：不继承
		可能的值：
			repeat：背景图像在水平和垂直位置重复
			repeat-x：在水平方向重复
			repeat-y：在垂直方向重复
			no-repeat：背景仅显示一次
			inherit：继承
	background-position：规定图像的位置
		默认值：0% 0%（即左上角）
		继承性：不继承
		可能的值：
			top center bottom和left center right共组成9种状态，如center center表示正中间
			x% y%：表示水平位置和垂直位置，若只规定一个值，另一个值表示50%
			xpos ypos：通过像素来表示位置，若只规定一个值，另一个值表示50%
	background-attachment：规定背景图像是否随页面滚动
		默认值：scroll
		继承性：不继承
		可能的值：
			scroll：背景图像会随着一起滚动（即背景图像会随着滚动被隐藏）
			fixed：即固定页面，背景图像不会滚动（即总是能看到背景图像）
			inherit：可继承

	text-indent：设置缩进大小
		默认值：没有
		继承性：继承
		可能的值：
			length：定义固定的缩进（可为负值）
			%：定义基于父元素宽度的百分比的缩进
			inherit：可继承
```
