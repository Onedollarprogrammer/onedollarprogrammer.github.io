---
layout : post
title : "Mysql常用总结"
category : DataBase
duoshuo: true
date : 2014-07-25
tags : [DataBase , Mysql ]
SyntaxHihglighter: true
shTheme: shThemeMidnight # shThemeDefault  shThemeDjango  shThemeEclipse  shThemeEmacs  shThemeFadeToGrey  shThemeMidnight  shThemeRDark
---

Mysql数据库常用语句总结

<!-- more -->

* **创建和查看数据库**
  create database ```数据库名称```  
  show databases;```查看所有数据库```  
  show create database ```指定数据库```  

* **修改数据库**  
  alter database ```数据库名称``` default character set ```编码方式``` collate ```编码方式_bin```;  
  eg:alter database db default character set **gbk** collate **gbk**_bin;  
  
* **删除数据库**  
  drop database ```数据库名称```;
  
* **查看数据表**  
  不仅可以查看数据表定义语句，还可以查看表的字符编码  
  show create table ```数据库表名```  
  
* **使用describe语句查看数据表**  
  可以查看表的字段信息，包括字段名、类型等信息。  
  describe ```数据库表名```  
  desc ```数据库表名```

* **修改数据库表名**  
  alter table ```旧表名``` rename [to] ```新表名```  
  eg:alter table old_table rename to new_table  

* **修改数据库表字段名**  
  alter table ```表名``` change ```旧字段名``` ```新字段名``` ```新数据类型```  
  eg:alter table grade change name username varchar(20);  

* **修改数据库表字段数据类型**  
  alter table ```表名``` modify ```字段名``` ```数据类型```  
  alter table grade modify username varchar(30);

* **添加字段**  
  alter table ```表名``` add ```新字段名``` ```数据类型``` 【约束条件】 【first|after ```已存在字段```】  
  eg:alter table grade add age int(10);  

* **删除字段**  
  alter table ```表名``` drop ```字段名```  
  eg:alter table grade drop age;
  
* **修改字段的排列位置**  
  alter table ```表名``` modify ```字段名1``` ```数据类型``` first|after ```字段名2```  
  eg:alter table grade modify age int after sex;
  
* **删除数据表**  
  drop table ```表名```  
  
* **单字段主键**  
  ```字段名``` ```数据类型``` primary key  
  eg:age int primary key;
  
* **多字段主键**  
  primary key(```字段名1```,```字段名2```,```字段名n```)  
  eg:primary key(```age```,```sex```,```id```);
  
* **非空约束**  
  ```字段名``` ```数据类型``` not null  
  
* **唯一约束**  
  ```字段名``` ```数据类型``` unique  
  
* **默认约束**  
  ```字段名``` ```数据类型``` default ```默认值```  
  eg:age int default 0;
  
* **设置表的字段值为自动增加**  
  ```字段名``` ```数据类型``` auto_increment  
  eg:age int auto_increment;
  
###添加/更新/删除数据

* **为表中所有字段添加数据**  
  ```指定字段名``` insert into ```表名```( ```字段名1```, ```字段名2```,```字段名3```) values(```值1```,```值2```,```值3```);  
  ```不指定字段名```insert into ```表名``` values(```值1```,```值2```,```值3```);  
  
* **为表中指定字段添加数据**  
	insert into ```表名```( ```字段名1```, ```字段名2```) values(```值1```,```值2```); 

* **insert语句的其他写法**  
	insert into ```表名``` set ```字段名1=值1```, ```字段名2=值2```  
