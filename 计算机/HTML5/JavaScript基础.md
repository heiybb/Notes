# JavaScript基础教程


## 一、基础语法

---

<script>元素


## 二、特殊用法

---

### 闭包


### 匿名函数

### DOM操作

```

```

特殊运算符（和C语言不同的）：
  ===：用来判断类型是否相同
	!==：用来判断类型是否不相同
	>>>：按位右移，左边补0

控制结构完全同C


调用外部js文件：<script type="text/javascript" src="file_name"></script>


特殊的函数调用方式：
	1、通过链接调用函数
		href="JavaScript:function_name()"
	2、从事件调用函数
		onClick="function_name()"
	3、从script中调用


Function对象：即把函数当作对象，这个实际上可以联想C的函数指针，但是它并不是个指针



匿名函数（实际上也是直接得益与Function对象）
	function_name = function(){}


javascript只有全局变量和局部变量之分，在非函数部分都是全局变量，在函数内部加上var才是局部变量（对，不加var依然是全局变量）


闭包（实际上都得益与Function对象）：
	C语言中不允许函数嵌套，但是javascript允许。
	一般情况下，任何语言都是只允许内部的函数访问外围数据，外部（当然包括javascript的外围嵌套函数）则无法使用内部函数的局部变量（包括var的Function对象），但是有时候又是需要方便的访问内部函数的局部变量的，此时闭包就起作用了，直接看下面的例子就什么都明白了

function f1(){
	var n=999;     // 局部变量
	nAdd=function(){n+=1}    // 全局变量
	function f2(){alert(n);}    // 局部变量
    return f2;
}
var result=f1();    // 执行f1()
result(); // 执行f2——alert(999)
nAdd();    // 执行nAdd()
result(); // 执行f2()——alert(1000)


在定义函数的时候，一定要加上(){}来对其限制，即使没有函数题内部没有语句，也要加上{}

try/throw/catch/finally：测试代码快/抛出异常/异常后的处理代码/无论是否异常后都要处理的代码

Javascript不如C++等语言对对象的支持那么强（毕竟只是个处理附属数据的脚本语言），但还是一定意义上支持对象的
	创建对象：
		var case_name = new object_name(par1, par2, ...)
	创建函数对象（注意后面的Function中F一定给要大写，参数和函数体一定要写成字符串形式）
		var function_name = new Function("par1", "par2", ... ,"fucntion sentence")
	Object对象：其它对象的基类，通过以下句子建立了一个新动态实例——可任意扩充属性和方法
					var case_name = new Object()




字符串用双引号包含，为了在其中包含特殊符号，需要用\符号，为了包含换行符，可以在要换行的地方加上\后换行



prototype原型实现机理，javascript对象机理，和C++以及Java比较

通过this实现number对象加法，如numberObj.add(number)

类方法、对象方法、原型方法


关于下面这段代码的理解


function People(name)
{
this.name=name;
//对象方法
this.Introduce=function(){
alert("My name is "+this.name);
}
}
//类方法
People.Run=function(){
alert("I can run");
}


//测试

var p1=new People("Windking");
p1.Introduce();
People.Run();

//原型方法
People.prototype.IntroduceChinese=function(){
alert("我的名字是"+this.name);
}

p1.IntroduceChinese();



## 方法

write()：
writeln()：

函数
alert()：弹出文本提示对话框
prompt()：弹出输入对话框
confirm()：弹出确认对话框
