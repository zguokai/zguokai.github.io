SockJS-based

在IE10以下版本可能没有实现WebSocket，所以，用SockJS-based


Building URIs to Controllers and methods from views


Executing SQL scripts

@Sql
@SqlConfig


java -DSERVER_PORT=9002 -jar .\target\com.ricequant-1.0-SNAPSHOT.war  
```
@Bean
	public EmbeddedServletContainerFactory servletContainer() {
		TomcatEmbeddedServletContainerFactory factory = new TomcatEmbeddedServletContainerFactory();
		factory.setPort(Integer.parseInt(System.getProperty("server.port", "9000")));
		//factory.setPort(9000);
		factory.setSessionTimeout(10, TimeUnit.MINUTES);
		factory.addErrorPages(new ErrorPage(HttpStatus.NOT_FOUND, "/notfound.jsp"));
		return factory;
	}
```

### Spring-boot-cli  
它也可以监控文件，当文件改变时，自动重新编译并重启


### Spring-bbot-actuator
它是高级的auto-configuration，可以用于监控应用运行时的各种参数。
http://spring.io/guides/gs/spring-boot/


### Session如何解决？  







