# DatabaseTablesToEntities
数据库表转实体 现支持mysql以及oracle

使用指南


1.首先配置需要生成实体所在的库

这个是mysql的模板 只需要将自己的配置填充就好

spring.mysql.jdbc-url=jdbc:mysql://127.0.0.1/test?useSSL=false&useUnicode=true&characterEncoding=UTF-8


spring.mysql.username=root


spring.mysql.password=root


spring.mysql.driver-class-name=com.mysql.jdbc.Driver

2.table_name.txt

在这个文本中配置需要转的表名，每个表明一行

如：


t_label


t_label_group

3.提供web接口调用生成实体

oracle/create 生成oracle表对应实体


mysql/create  生成mysql表对应实体

实体生成的路径在src.main.java.com.rain.model这个目录下

4.数据库表可配置前缀

如：

table.prefix = t           t为前缀  

当表没有前缀的时候       前缀配置为      table.prefix = null


有的朋友maven没有oracle的依赖  在lib中有oracle的jar包 和手动安装命令  如有需要可以手动安装   


有的已经maven已有了oracle依赖  请把pom中的依赖替换成 你的版本 







！！！！花了一天写的，恳请大佬们指点，要是有其他数据源，希望不吝添加，谢谢！




加了一点彩蛋 。。。启动图标要是不喜欢 初音未来 可以把上个目录的banner.txt替换掉resource下的banner.txt  孙悟空哦！！
