## Spring常用依赖

```xml

<dependency>
    <groupId>org.springframework</groupId>
    <artifactId>spring-webmvc</artifactId>
    <version>5.2.11.RELEASE</version>
</dependency>
<dependency>
<groupId>junit</groupId>
<artifactId>junit</artifactId>
<version>4.12</version>
<scope>test</scope>
</dependency>
```
##注解方式
- @Autowired:自动装配通过类型。名字
    如果Autowired不能唯一自动装配配上属性，则需要通过@Qualifier(value="xxx")
- @Nullable  字段标记了这个注解，说明这个字段可以为Null;  
- @Resource:自动装配先通过名字再去类型
- @Component:组件，放在类上，说明这个类被Spring管理了，就是Bean!
   有几个衍生的注解，我们在web开发中，会按照mvc三层架构分层！
   dao[@Repository]
   service[@Service]
   controller[@Controller]
  这四个注解功能都是一样的，都是代表将某个类注册到Spring中，装配Bean