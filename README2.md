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

## 中级

### 简单JPA生成代码

### 目录命名规则

### 增量开发流程

#### liquibase增加字段

#### profile的使用方式

## 高级

### docker启动

### kafka

    Parameter 0 of constructor in com.sgcc.syn.messaging.ProducerResource required a bean of type 'com.sgcc.syn.messaging.ProducerChannel' that could not be found.

在 MessagingConfiguration 类里

    @EnableBinding(value = {Source.class, ProducerChannel.class, ConsumerChannel.class})
    public class MessagingConfiguration {

    }
    

### websocket

### cache缓存