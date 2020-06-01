##基本命令

  ***
进入数据库:
`mysql -uroot -p  `
//输入密码 15793  
  ***
`show databases;`//显示所有数据库名称  
  ***
`use ____(数据库名字)`//进入数据库 
***
创建数据库  
 `create table ______(数据库名称)`  
`(Sno CHAR(9)PRIMARY KEY, //唯一主码`  
`Sname CHAR(20) UNIQUE, //取值唯一`  
`Sage SMALLINT //结尾不带,号`  
`);`  
***

 显示所有表    
`show tables;`
***
显示表结构  
`desc _____(table名)`
***
选择数据库   
`use _______(database_name)`
***
删除数据库   
`DROP TABLE ____(table_name)`
***
向表中插入数据  
`insert into ____(表名) values`  
`("数据",//此处都为单引号 "数据","数据"),`   
`("数据",//此处都为单引号 "数据","数据"),`   
`("数据",//此处都为单引号 "数据","数据");`   //根据数据格式取决用不用引号  
***
查询数据   
`SELECT column_name,column_name`   
`FROM table_name`   
`WHERE xxxx`
   
`SELECT * FORM _____(table_name)`
***  
UPDATE更新  
`UPDATE ___(table_name) SET field1=new-value1,field2=new-value2`
***  
