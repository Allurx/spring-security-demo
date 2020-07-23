## 涉及技术
### 认证令牌
[jwt](https://jwt.io/)
### 接口文档
[swagger-ui](https://swagger.io/tools/swagger-ui/)
### 用户存储
[redis](https://redis.io/)
## 版本信息
### spring-boot
```xml
<parent>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-parent</artifactId>
    <version>2.1.5.RELEASE</version>
</parent>
```
### mysql
```
8.0.13
```
### jdk
```
1.8
```
## 运行
### 创建数据库
创建一个名称为spring-security-demo的mysql数据库，然后执行[spring-security-demo.sql](https://github.com/Allurx/spring-security-demo/blob/master/src/main/resources/spring-security-demo.sql
)这个sql脚本初始化表结构
### 访问swagger
启动项目，在浏览器访问`localhost:9000/swagger-ui.html`即可看到swagger页面
### 用户登录
选择登陆接口，默认的三个用户（admin，user1，user2）的密码都是123456
### 测试接口
点击swagger右上角的Authorize按钮，将登陆返回的token信息填入，然后对相应的接口进行认证权限测试
### spring-security源码解析
[spring-security源码解析](https://www.zyc.red/categories/Spring/Spring-Security/)
