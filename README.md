### 项目介绍

这是一个Spring+MyBatis开发整合包，开箱即用。

### 使用前应注意

1、使用IntelliJ IDEA导入该整合包。

2、确保lib文件夹中的所有依赖JAR包已经全部“添加为库”。

3、确保resources已经被标记为“资源根目录”。

### 配置说明

1、classpath:log4j.properties：LOG4J日志配置，一般不需要改。

2、classpath:applicationContext.xml：Spring核心配置文件，需要修改数据库连接信息和注解扫包。

3、classpath:mybatis-config.xml：MyBatis配置文件，需要修改SQL映射文件扫包。

### 编码过程

1、创建数据库表对应的实体类。

2、创建数据库表对应的Mapper接口和SQL映射文件。

3、在SQL映射文件中编写相关SQL语句。

4、创建Service接口和实现类，Service实现类上必须添加@Service注解。

5、在Service实现类中调用Mapper中的方法，Service实现类中使用@Resource注解注入Mapper。

6、编写测试类和测试方法，从Spring容器中获取Service Bean对象，并调用Service方法。
