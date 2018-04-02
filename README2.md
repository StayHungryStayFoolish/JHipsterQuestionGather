## 初级

### 确定版本

    ➜  ~ jhipster --version
    Using JHipster version installed globally
    4.14.1

### 加速三步骤

#### pom.xml

  [阿里云代理](https://www.cnblogs.com/xinhudong/p/7804968.html)

#### nodejs 代理

  [npm 淘宝](https://npm.taobao.org/)

#### pathmanjs 迅雷下载

    yarn start 过程中 会下载 phantomjs-2.1.1-macosx.zip包，该包体积较大，国内仅能从迅雷下载，然后拷贝到对应目录中
    
<img src="https://github.com/StayHungryStayFoolish/Images-Blog/blob/master/jhipster/1522214654527.jpg?raw=true" />    

## 中级

### 简单JPA生成代码

#### 根据表 生成实体

  jhipster entity <entityName> --[options]

### 目录命名规则

### 增量开发流程

[database-updates-with-the-maven-liquibasediff-goal](http://www.jhipster.tech/development/#database-updates-with-the-maven-liquibasediff-goal)

#### 数据库更新 三种工作方式

#### 1、以entity sub-generator方式

#### 2、以liquibase:diff goal方式

#### 3、以编辑change log文件(修改字段...)方式

* 修改JPA实体(添加字段、修改关系)

* 新建 "change log"文件 如:20141006152300_added_price_to_product.xml

* 将上一步文件放到 master.xml文件中，重启生效。

#### profile的使用方式

### 角色与授权

[add ROLE_MANAGER](https://stackoverflow.com/questions/32436745/using-roles-in-jhipster)

[Spring Data REST + Spring Security](https://github.com/spring-projects/spring-data-examples/tree/master/rest/security)

## 高级

### docker启动

### kafka

* 程序启动报错

    Parameter 0 of constructor in com.sgcc.syn.messaging.ProducerResource required a bean of type 'com.sgcc.syn.messaging.ProducerChannel' that could not be found.

在 MessagingConfiguration 类里

    @EnableBinding(value = {Source.class, ProducerChannel.class, ConsumerChannel.class})
    public class MessagingConfiguration {

    }

* 消息未订阅成功

配置文件 application-dev.yml 添加以下内容

    bindings:
                messageChannel:
                    destination: greetings
                    content-type: application/json
                subscribableChannel:
                    destination: greetings
    

### websocket

### cache缓存
