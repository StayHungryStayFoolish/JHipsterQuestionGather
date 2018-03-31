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

### 目录命名规则

### 增量开发流程

[database-updates-with-the-maven-liquibasediff-goal](http://www.jhipster.tech/development/#database-updates-with-the-maven-liquibasediff-goal)

### 数据库已经存在重新生成代码

#### liquibase增加字段

#### profile的使用方式

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
