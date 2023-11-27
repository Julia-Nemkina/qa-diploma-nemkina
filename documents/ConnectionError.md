PS J:\Projects_for_Netology\qa-diploma-nemkina> java -jar .\aqa-shop.jar

.   ____          _            __ _ _
/\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
\\/  ___)| |_)| | | | | || (_| |  ) ) ) )
'  |____| .__|_| |_|_| |_\__, | / / / /
=========|_|==============|___/=/_/_/_/
:: Spring Boot ::        (v2.2.1.RELEASE)

2023-11-27 21:28:54.662  INFO 20152 --- [           main] ru.netology.shop.ShopApplication         : Starting ShopApplication v0.0.1-SNAPSHOT on Vincent with PID 2
0152 (J:\Projects_for_Netology\qa-diploma-nemkina\aqa-shop.jar started by ▐ыш  in J:\Projects_for_Netology\qa-diploma-nemkina)
2023-11-27 21:28:54.670  INFO 20152 --- [           main] ru.netology.shop.ShopApplication         : No active profile set, falling back to default profiles: defau
lt
2023-11-27 21:28:56.615  INFO 20152 --- [           main] .s.d.r.c.RepositoryConfigurationDelegate : Bootstrapping Spring Data repositories in DEFAULT mode.
2023-11-27 21:28:56.820  INFO 20152 --- [           main] .s.d.r.c.RepositoryConfigurationDelegate : Finished Spring Data repository scanning in 184ms. Found 3 rep
ository interfaces.
2023-11-27 21:28:57.828  INFO 20152 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'org.springframework.transaction.annotation.ProxyTransact
ionManagementConfiguration' of type [org.springframework.transaction.annotation.ProxyTransactionManagementConfiguration] is not eligible for getting processed by a
ll BeanPostProcessors (for example: not eligible for auto-proxying)
2023-11-27 21:28:59.269  INFO 20152 --- [           main] o.s.b.w.embedded.tomcat.TomcatWebServer  : Tomcat initialized with port(s): 8080 (http)
2023-11-27 21:28:59.293  INFO 20152 --- [           main] o.apache.catalina.core.StandardService   : Starting service [Tomcat]
2023-11-27 21:28:59.293  INFO 20152 --- [           main] org.apache.catalina.core.StandardEngine  : Starting Servlet engine: [Apache Tomcat/9.0.27]
2023-11-27 21:28:59.458  INFO 20152 --- [           main] o.a.c.c.C.[Tomcat].[localhost].[/]       : Initializing Spring embedded WebApplicationContext
2023-11-27 21:28:59.460  INFO 20152 --- [           main] o.s.web.context.ContextLoader            : Root WebApplicationContext: initialization completed in 4587 m
s
2023-11-27 21:29:00.111  INFO 20152 --- [           main] o.hibernate.jpa.internal.util.LogHelper  : HHH000204: Processing PersistenceUnitInfo [name: default]
2023-11-27 21:29:00.368  INFO 20152 --- [           main] org.hibernate.Version                    : HHH000412: Hibernate Core {5.4.8.Final}
2023-11-27 21:29:00.774  INFO 20152 --- [           main] o.hibernate.annotations.common.Version   : HCANN000001: Hibernate Commons Annotations {5.1.0.Final}
2023-11-27 21:29:01.008  INFO 20152 --- [           main] com.zaxxer.hikari.HikariDataSource       : HikariPool-1 - Starting...
2023-11-27 21:29:01.047  WARN 20152 --- [           main] o.h.e.j.e.i.JdbcEnvironmentInitiator     : HHH000342: Could not obtain connection to query metadata : Dri
ver org.h2.Driver claims to not accept jdbcUrl, jdbc:mysql//localhost:3306/app
2023-11-27 21:29:01.058  WARN 20152 --- [           main] ConfigServletWebServerApplicationContext : Exception encountered during context initialization - cancelli
ng refresh attempt: org.springframework.beans.factory.BeanCreationException: Error creating bean with name 'entityManagerFactory' defined in class path resource [o
rg/springframework/boot/autoconfigure/orm/jpa/HibernateJpaConfiguration.class]: Invocation of init method failed; nested exception is org.hibernate.service.spi.Ser
viceException: Unable to create requested service [org.hibernate.engine.jdbc.env.spi.JdbcEnvironment]
2023-11-27 21:29:01.074  INFO 20152 --- [           main] o.apache.catalina.core.StandardService   : Stopping service [Tomcat]
2023-11-27 21:29:01.101  INFO 20152 --- [           main] ConditionEvaluationReportLoggingListener :

Error starting ApplicationContext. To display the conditions report re-run your application with 'debug' enabled.
2023-11-27 21:29:01.120 ERROR 20152 --- [           main] o.s.boot.SpringApplication               : Application run failed

org.springframework.beans.factory.BeanCreationException: Error creating bean with name 'entityManagerFactory' defined in class path resource [org/springframework/b
oot/autoconfigure/orm/jpa/HibernateJpaConfiguration.class]: Invocation of init method failed; nested exception is org.hibernate.service.spi.ServiceException: Unabl
e to create requested service [org.hibernate.engine.jdbc.env.spi.JdbcEnvironment]
at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.initializeBean(AbstractAutowireCapableBeanFactory.java:1803) ~[spring-beans
-5.2.1.RELEASE.jar!/:5.2.1.RELEASE]
at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.doCreateBean(AbstractAutowireCapableBeanFactory.java:595) ~[spring-beans-5.
2.1.RELEASE.jar!/:5.2.1.RELEASE]
at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.createBean(AbstractAutowireCapableBeanFactory.java:517) ~[spring-beans-5.2.
1.RELEASE.jar!/:5.2.1.RELEASE]
at org.springframework.beans.factory.support.AbstractBeanFactory.lambda$doGetBean$0(AbstractBeanFactory.java:323) ~[spring-beans-5.2.1.RELEASE.jar!/:5.2.1.
RELEASE]
at org.springframework.beans.factory.support.DefaultSingletonBeanRegistry.getSingleton(DefaultSingletonBeanRegistry.java:222) ~[spring-beans-5.2.1.RELEASE.
jar!/:5.2.1.RELEASE]
at org.springframework.beans.factory.support.AbstractBeanFactory.doGetBean(AbstractBeanFactory.java:321) ~[spring-beans-5.2.1.RELEASE.jar!/:5.2.1.RELEASE]
at org.springframework.beans.factory.support.AbstractBeanFactory.getBean(AbstractBeanFactory.java:202) ~[spring-beans-5.2.1.RELEASE.jar!/:5.2.1.RELEASE]   
at org.springframework.context.support.AbstractApplicationContext.getBean(AbstractApplicationContext.java:1108) ~[spring-context-5.2.1.RELEASE.jar!/:5.2.1.
RELEASE]
at org.springframework.context.support.AbstractApplicationContext.finishBeanFactoryInitialization(AbstractApplicationContext.java:868) ~[spring-context-5.2
.1.RELEASE.jar!/:5.2.1.RELEASE]
at org.springframework.context.support.AbstractApplicationContext.refresh(AbstractApplicationContext.java:550) ~[spring-context-5.2.1.RELEASE.jar!/:5.2.1.R
ELEASE]
at org.springframework.boot.web.servlet.context.ServletWebServerApplicationContext.refresh(ServletWebServerApplicationContext.java:141) ~[spring-boot-2.2.1
.RELEASE.jar!/:2.2.1.RELEASE]
at org.springframework.boot.SpringApplication.refresh(SpringApplication.java:747) ~[spring-boot-2.2.1.RELEASE.jar!/:2.2.1.RELEASE]
at org.springframework.boot.SpringApplication.refreshContext(SpringApplication.java:397) ~[spring-boot-2.2.1.RELEASE.jar!/:2.2.1.RELEASE]
at org.springframework.boot.SpringApplication.run(SpringApplication.java:315) ~[spring-boot-2.2.1.RELEASE.jar!/:2.2.1.RELEASE]
at org.springframework.boot.SpringApplication.run(SpringApplication.java:1226) ~[spring-boot-2.2.1.RELEASE.jar!/:2.2.1.RELEASE]
at org.springframework.boot.SpringApplication.run(SpringApplication.java:1215) ~[spring-boot-2.2.1.RELEASE.jar!/:2.2.1.RELEASE]
at ru.netology.shop.ShopApplication.main(ShopApplication.java:10) ~[classes!/:0.0.1-SNAPSHOT]
at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[na:na]
at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[na:na]
at java.base/jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[na:na]
at java.base/java.lang.reflect.Method.invoke(Method.java:566) ~[na:na]
at org.springframework.boot.loader.MainMethodRunner.run(MainMethodRunner.java:48) ~[aqa-shop.jar:0.0.1-SNAPSHOT]
at org.springframework.boot.loader.Launcher.launch(Launcher.java:87) ~[aqa-shop.jar:0.0.1-SNAPSHOT]
at org.springframework.boot.loader.Launcher.launch(Launcher.java:51) ~[aqa-shop.jar:0.0.1-SNAPSHOT]
at org.springframework.boot.loader.JarLauncher.main(JarLauncher.java:52) ~[aqa-shop.jar:0.0.1-SNAPSHOT]
Caused by: org.hibernate.service.spi.ServiceException: Unable to create requested service [org.hibernate.engine.jdbc.env.spi.JdbcEnvironment]
at org.hibernate.service.internal.AbstractServiceRegistryImpl.createService(AbstractServiceRegistryImpl.java:275) ~[hibernate-core-5.4.8.Final.jar!/:5.4.8.
Final]
at org.hibernate.service.internal.AbstractServiceRegistryImpl.initializeService(AbstractServiceRegistryImpl.java:237) ~[hibernate-core-5.4.8.Final.jar!/:5.
4.8.Final]
at org.hibernate.service.internal.AbstractServiceRegistryImpl.getService(AbstractServiceRegistryImpl.java:214) ~[hibernate-core-5.4.8.Final.jar!/:5.4.8.Fin
al]
at org.hibernate.id.factory.internal.DefaultIdentifierGeneratorFactory.injectServices(DefaultIdentifierGeneratorFactory.java:152) ~[hibernate-core-5.4.8.Fi
nal.jar!/:5.4.8.Final]
at org.hibernate.service.internal.AbstractServiceRegistryImpl.injectDependencies(AbstractServiceRegistryImpl.java:286) ~[hibernate-core-5.4.8.Final.jar!/:5
.4.8.Final]
at org.hibernate.service.internal.AbstractServiceRegistryImpl.initializeService(AbstractServiceRegistryImpl.java:243) ~[hibernate-core-5.4.8.Final.jar!/:5.
4.8.Final]
at org.hibernate.service.internal.AbstractServiceRegistryImpl.getService(AbstractServiceRegistryImpl.java:214) ~[hibernate-core-5.4.8.Final.jar!/:5.4.8.Fin
al]
at org.hibernate.boot.internal.InFlightMetadataCollectorImpl.<init>(InFlightMetadataCollectorImpl.java:175) ~[hibernate-core-5.4.8.Final.jar!/:5.4.8.Final]
at org.hibernate.boot.model.process.spi.MetadataBuildingProcess.complete(MetadataBuildingProcess.java:118) ~[hibernate-core-5.4.8.Final.jar!/:5.4.8.Final]
at org.hibernate.jpa.boot.internal.EntityManagerFactoryBuilderImpl.metadata(EntityManagerFactoryBuilderImpl.java:1214) ~[hibernate-core-5.4.8.Final.jar!/:5
.4.8.Final]
at org.hibernate.jpa.boot.internal.EntityManagerFactoryBuilderImpl.build(EntityManagerFactoryBuilderImpl.java:1245) ~[hibernate-core-5.4.8.Final.jar!/:5.4.
8.Final]
at org.springframework.orm.jpa.vendor.SpringHibernateJpaPersistenceProvider.createContainerEntityManagerFactory(SpringHibernateJpaPersistenceProvider.java:
58) ~[spring-orm-5.2.1.RELEASE.jar!/:5.2.1.RELEASE]
    at org.springframework.orm.jpa.LocalContainerEntityManagerFactoryBean.createNativeEntityManagerFactory(LocalContainerEntityManagerFactoryBean.java:365) ~[s
    pring-orm-5.2.1.RELEASE.jar!/:5.2.1.RELEASE]
    at org.springframework.orm.jpa.AbstractEntityManagerFactoryBean.buildNativeEntityManagerFactory(AbstractEntityManagerFactoryBean.java:391) ~[spring-orm-5.2
    .1.RELEASE.jar!/:5.2.1.RELEASE]
    at org.springframework.orm.jpa.AbstractEntityManagerFactoryBean.afterPropertiesSet(AbstractEntityManagerFactoryBean.java:378) ~[spring-orm-5.2.1.RELEASE.ja
    r!/:5.2.1.RELEASE]
    at org.springframework.orm.jpa.LocalContainerEntityManagerFactoryBean.afterPropertiesSet(LocalContainerEntityManagerFactoryBean.java:341) ~[spring-orm-5.2.
    1.RELEASE.jar!/:5.2.1.RELEASE]
    at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.invokeInitMethods(AbstractAutowireCapableBeanFactory.java:1862) ~[spring-be
    ans-5.2.1.RELEASE.jar!/:5.2.1.RELEASE]
    at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.initializeBean(AbstractAutowireCapableBeanFactory.java:1799) ~[spring-beans
    -5.2.1.RELEASE.jar!/:5.2.1.RELEASE]
    ... 24 common frames omitted
    Caused by: org.hibernate.HibernateException: Access to DialectResolutionInfo cannot be null when 'hibernate.dialect' not set
    at org.hibernate.engine.jdbc.dialect.internal.DialectFactoryImpl.determineDialect(DialectFactoryImpl.java:100) ~[hibernate-core-5.4.8.Final.jar!/:5.4.8.Fin
    al]
    at org.hibernate.engine.jdbc.dialect.internal.DialectFactoryImpl.buildDialect(DialectFactoryImpl.java:54) ~[hibernate-core-5.4.8.Final.jar!/:5.4.8.Final]  
    at org.hibernate.engine.jdbc.env.internal.JdbcEnvironmentInitiator.initiateService(JdbcEnvironmentInitiator.java:137) ~[hibernate-core-5.4.8.Final.jar!/:5.
    4.8.Final]
    at org.hibernate.engine.jdbc.env.internal.JdbcEnvironmentInitiator.initiateService(JdbcEnvironmentInitiator.java:35) ~[hibernate-core-5.4.8.Final.jar!/:5.4
    .8.Final]
    at org.hibernate.boot.registry.internal.StandardServiceRegistryImpl.initiateService(StandardServiceRegistryImpl.java:101) ~[hibernate-core-5.4.8.Final.jar!
    /:5.4.8.Final]
    at org.hibernate.service.internal.AbstractServiceRegistryImpl.createService(AbstractServiceRegistryImpl.java:263) ~[hibernate-core-5.4.8.Final.jar!/:5.4.8.
    Final]
    ... 41 common frames omitted
