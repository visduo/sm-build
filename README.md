### 项目介绍

这是一个 Spring + MyBatis 开发整合包，开箱即用。

### 使用前应注意

1、使用 IntelliJ IDEA 导入该整合包。

2、确保 lib 文件夹中的所有依赖 JAR 包已经全部添加为库。

3、确保 resources 文件夹已经被标记为资源根目录。

4、确保 src 文件夹已经被标记为源代码根目录。

### 配置说明

1、classpath:log4j.properties：LOG4J 日志配置，一般不需要改。

2、classpath:applicationContext.xml：Spring 核心配置文件，需要修改数据库连接信息和注解扫包。

3、classpath:mybatis-config.xml：MyBatis 配置文件，需要修改 SQL 映射文件扫包。

### 编码过程

1、创建数据库表对应的实体类。

2、创建数据库表对应的 Mapper 接口和 SQL 映射文件。

3、在SQL映射文件中编写相关 SQL 语句。

4、创建 Service 接口和实现类，Service 实现类上必须添加 @Service 注解。

5、在 Service 实现类中调用 Mapper 中的方法，Service 实现类中使用 @Resource 注解注入 Mapper。

6、编写测试类和测试方法，从 Spring 容器中获取 Service Bean 对象，并调用 Service 方法。
