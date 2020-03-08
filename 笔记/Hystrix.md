#Hystrix实现步骤
##1.导入依赖
```xml
<!--Hystrix依赖-->
<dependency>
    <groupId>org.springframework.cloud</groupId>
    <artifactId>spring-cloud-starter-hystrix</artifactId>
    <version>1.4.6.RELEASE</version>
</dependency>
```

##2.在要熔断的类上指定熔断解决方案
@HystrixCommand(fallbackMethod = "类名")


##3.在主应用程序加上@EnableCircuitBreaker注解，开启对熔断的支持