# SQL 简介

结构化查询语言(Structured Query Language)简称SQL，是一种数据库查询和程序设计语言，用于存取数据以及查询、更新和管理关系数据库系统。

创建数据库、创建数据表、向数据表中添加一条条数据信息均需要使用SQL语句。

# SQL 语句
## SQL 分类
    数据定义语言：简称DDL(Data Definition Language)，用来定义数据库对象：数据库，表，列等。关键字：create，alter，drop等 
    数据操作语言：简称DML(Data Manipulation Language)，用来对数据库中表的记录进行更新。关键字：insert，delete，update等
    数据控制语言：简称DCL(Data Control Language)，用来定义数据库的访问权限和安全级别，及创建用户。
    数据查询语言：简称DQL(Data Query Language)，用来查询数据库中表的记录。关键字：select，from，where等
    
## SQL 通用语法
- SQL语句可以单行或多行书写，以分号结尾
- 可使用空格和缩进来增强语句的可读性
- MySQL数据库的SQL语句不区分大小写，建议使用大写，例如：SELECT * FROM user。
- 同样可以使用/**/的方式完成注释
- MySQL中的我们常使用的数据类型如下

![image](https://user-images.githubusercontent.com/34376972/146479188-75896eae-b38b-4b99-bf76-63b33e1c84ca.png)

|分类	| 类型名称 |	说明 |
|---|---|---|
|整数类型 | tinyInt |	很小的整数|
| |	smallint | 小的整数|
|	|mediumint	| 中等大小的整数|
|	|int(integer)	| 普通大小的整数|
|小数类型	| float	| 单精度浮点数|
|	| double | 双精度浮点数|
|	|decimal（m,d）| 压缩严格的定点数|
|日期类型	| year | YYYY | 1901~2155|
| |time | HH:MM:SS | -838:59:59~838:59:59|
| |date	| YYYY-MM-DD | 1000-01-01~9999-12-3|
| |datetime | YYYY-MM-DD HH:MM:SS | 1000-01-01 00:00:00~ 9999-12-31 23:59:59|
| |timestamp | YYYY-MM-DD HH:MM:SS | 1970~01~01 00:00:01 UTC~2038-01-19 03:14:07UTC|
|文本、二进制类型	| CHAR(M) | M为0~255之间的整数|
| |VARCHAR(M)	| M为0~65535之间的整数|
| |TINYBLOB | 允许长度0~255字节|
| |BLOB | 允许长度0~65535字节|
| |MEDIUMBLOB | 允许长度0~167772150字节|
| |LONGBLOB | 允许长度0~4294967295字节|
| |TINYTEXT | 允许长度0~255字节|
| |TEXT | 允许长度0~65535字节|
| |MEDIUMTEXT	| 允许长度0~167772150字节|
| |LONGTEXT | 允许长度0~4294967295字节|
| |VARBINARY(M) | 允许长度0~M个字节的变长字节字符串|
| |BINARY(M) | 允许长度0~M个字节的定长字节字符串|

## 数据库操作
### 创建数据库
- 格式:
    * create database 数据库名;
    * create database 数据库名 character set 字符集;
- 例如：
    * 创建数据库 数据库中数据的编码采用的是安装数据库时指定的默认编码 utf8
      CREATE DATABASE day21_1; 
    * 创建数据库 并指定数据库中数据的编码
      CREATE DATABASE day21_2 CHARACTER SET utf8;
      
![image](https://user-images.githubusercontent.com/34376972/146481802-cb3cb208-538b-467e-bc3e-94ddef36c6d2.png)








