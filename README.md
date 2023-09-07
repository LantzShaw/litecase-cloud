# litecase cloud


### Record

**spring cloud**

```shell
服务注册中心 server
服务提供者 client
服务调用 feign
服务网关 gateway zuul
服务配置中心 config
服务熔断
```

**spring cloud config 多环境配置**
```text
https://juejin.cn/post/6997031315425984548
```

**gson报错，slf4j依赖报错 需要引入spring-boot-starter-parent以及spring-boot-starter-web**

```shell
# 以下这些都不用单独引入
# server
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot</artifactId>
    <version>3.1.0</version>
    <scope>compile</scope>
</dependency>
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-autoconfigure</artifactId>
    <version>3.1.0</version>
    <scope>compile</scope>
</dependency>
<dependency>
    <groupId>com.google.code.gson</groupId>
    <artifactId>gson</artifactId>
    <version>2.9.1</version>
</dependency>

# client

<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-autoconfigure</artifactId>
    <version>3.1.0</version>
</dependency>
<dependency>
    <groupId>com.google.code.gson</groupId>
    <artifactId>gson</artifactId>
    <version>2.9.1</version>
</dependency>

```