### 极客时间课后作业

#### 第一周

##### 作业运行说明

```shell
mvn clean package -U
java -jar .\user-web\target\user-web-v1-SNAPSHOT-war-exec.jar
```

运行成功后，可访问 http://localhost:8080/register-form 注册用户

注册成功后跳转至登录页 http://localhost:8080/login-form 进行登录

登录成功会forward到登录成功的提示页，若用户名或密码错误则forward到错误提示页

内部使用JNDI和ServletContextListener初始化获取数据库连接

