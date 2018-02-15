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
