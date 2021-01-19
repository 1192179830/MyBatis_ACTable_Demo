A.CTable开源框架Mybatis增强自动创建表/更新表结构/实现类似hibernate共通的增删改查
项目结构：
<br>com.example -<br>
         config : 下面放一些mybatis的配置，默认都不需要修改 <br>
                      MybatisTableConfig.java  里面60行代码只需要修改一下包结构就可以  <br>   entity : 实体类，<br>
         mapper ： 映射类，可以不用管<br>
         vo     : 测试实体类，其中Test、Test1、UserLogin[MyBatisPlus]为三种方式<br>
        DemoApplication :启动类<br>

application .yml 配置 数据源！，特别注意需要来链接的数据库一定要创建好并打开
注意：若创建的SQL中的字段不全，则需要参考VO类中的Admin.java 
 在类上面添加 @Table (isSimple = true) 注解
