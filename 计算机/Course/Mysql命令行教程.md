# Mysql命令行教程


#### 开启mysql引擎服务程序（注意使用权限）：
    $(installLocation)/bin/mysqld：直接运行模式
    $(installLocation)/bin/mysqld_safe：安全模式下运行，默认运行模式



#### mysql：以当前用户访问，后面接数据库名称
    -u：后接用户名
    -p：直接输密码


#### 默认数据库
    mysql：重要数据库
        user：存储用户信息的表
  	

#### 确定使用数据库
    use mysql_name;
	

#### 显示所有当前用户可使用的数据库
    show databases;
	

#### 显示当前用户对各数据库的权限
    show grants;


#### 显示当前数据库中的表
    show tables;

#### 设置密码
    SET PASSWORD FOR 'root'@'localhost' = PASSWORD('newpwd');
	
	
