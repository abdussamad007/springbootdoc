**------************--------------**
**API used in Springboot start up **
**--------*****************-------**
-org.springframework.boot.SpringApplicationRunListener
	--Listener for the SpringApplication run method. 
		SpringApplicationRunListeners are loaded via the SpringFactoriesLoader and should declare a public constructor 
		that accepts a SpringApplication instance and a String[] of arguments. 
		A new SpringApplicationRunListener instance will be created for each run.

-org.springframework.web.context.support.StandardServletEnvironment		
	--Environment implementation to be used by Servlet-based web applications. 
		All web-related (servlet-based) ApplicationContext classes initialize an instance by default.
-org.springframework.core.env.StandardEnvironment
	--Environment implementation suitable for use in 'standard' (i.e. non-web) applications.
-org.springframework.boot.ConfigurableApplicationContext
	--Provides facilities to configure an application context in addition to the application context client 
		methods in the ApplicationContext interface.
-org.springframework.bootSpringApplication	
	--Classes that can be used to bootstrap and launch a Spring application from a Java main method. 
-org.springframework.boot.context.embedded.EmbeddedWebApplicationContext
	--This context will create, initialize and run an EmbeddedServletContainer by searching for a single 
	  EmbeddedServletContainerFactory bean within the ApplicationContext itself. 
	  The EmbeddedServletContainerFactory is free to use standard Spring concepts 
	  (such as dependency injection, lifecycle callbacks and property placeholder variables).
-org.springframework.boot.context.event.ApplicationFailedEvent
	--Event published by a SpringApplication when it fails to start.
