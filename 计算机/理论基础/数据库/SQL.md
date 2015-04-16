一、基本概念
  SQL全名结构化查询语言，是关系数据库国际标准语言，集数据库定义语言DDL、数据库操纵语言DML、数据控制语言DCL于一身，SQL即有关系代数的特点，又有关系演算的特点

二、SQL的特点
	综合统一
	高度非过程化
	面向集合的操作方式
	以同一种语法结构提供多种使用方式
	语言简洁

三、四大核心功能
	数据定义：Create、Drop、Alter
	数据查询：Select
	数据操纵：Insert、Update、Delete
	数据控制：Grant、Revoke
	
四、数据定义


五、数据查询
	select [all/distinct] <目标列表达式> [别名][,<目标列表达式> [别名]...]
	from 表名或视图名 [别名][,<表名或视图名> [别名]...]
	[where <条件表达式>]
	[group by <列名1> [having <条件表达式>]]
	[order by <列名2> [asc/desc]]