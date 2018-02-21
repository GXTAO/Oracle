Oracle:
JAVA程序存储数据：
    变量、数组、集合：数据仅仅保存在内存中。
    文件（file）    ：永久保存数据
        纯文件保存数据的缺点：
            1）只有一种数据类型
            2）没有访问安全限制
            3）数据量比较小
            4）没有提供备份恢复机制
            ......
    数据库：
        关系型数据库
            对数据进行存储、操作等管理。
            Oracle MySQL
        非关系型数据库
            Redis     key--value
            MOngoDB   nosql
        Oracle
            1.数据存放在表中(Table)
            2.Oracle中表数据是分用户管理的
            3.

         注意：1.安装Oracle..(tomact),目录中不能有中文
               2.必须保证Oracle的相关服务  启动状态
                OracleServeiceXE: Oracle核心服务
                OracleXEINSListener: 对外启动连接访问
               3.服务器端

                 客户端  1. sqlplus: dos界面
                               用户名：
                               密码：     
                                    -->登录
                          查看表结构：
                                desc 表名
                         2.web界面客户端
                                http://localhost:8080/apex
                         3.PLSQL Develpoer
                            输入用户名：
                            密码
                            数据库实例名
                            身份：normal
                                文件-新建-命令窗口
    SQL:结构化的查询语言
        select  name1,name2 from Table
        语法：
            select    from
                select:指定查看属性  from:指定属性所属表(Table)
                1.查看部分列 seclect name1,name2,.. from Table
                2.查看所有列 select from Table;/select * from Table
                3.对列的数据进行运算 select name1,name2,salary*12 from Table
                4.查询列名 更改
       排序
            1)多列排序
                select name1,name2 from Table order by name1,name3 desc;
            2)单列查询
                select name1,name2 from Table order by name1 desc;
       条件查询
            select 列1，列2 from Table where 过滤条件 order by 列 asc|desc;
            1)等值判断(=1000)
                select name1,name2 from Table where name3=1000;
            2)多条件
                select name1,name2 from Table where name1=1000 and name2*...;
            3)不等值查询
                select  name from Table where name<=1000 and name2>1000;
            4)区间查询between and
                select name between 5000 and 1000;
            5)空值处理
                select name from Table where name is null;
            6)枚举查询
                select * from Table where name1=** or name2=**;
                select * from Table where name1 in (**~**);
            NOTE:二者效率差别
           *7)模糊查询(查询名字是以K开头的员工):通配符 _:任一个、%:任多个
                select name1 from Table where name like 'K%'/'K___';(name's
                length)
       函数
            sysdate 系统时间(Y-M-D H-M-D weekend)
            dual:虚表  用于维护sql语句的完整
            select sysdate from dual;

                
