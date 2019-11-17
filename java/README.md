# Java

## Java

### Java Links:

The Java Tutorials from Oracle - https://docs.oracle.com/javase/tutorial/  
W3 schools - https://www.w3schools.com/java/  
Java Tutorial for Beginners video - https://www.youtube.com/watch?v=eIrMbAQSU34  
Learn Java 8 for Beginners video- https://www.youtube.com/watch?v=grEKMHGYyns  
Tutorial Point - https://www.tutorialspoint.com/java/index.htm  


Java EE  is a specification, EE = Java SE + components like JMS, Servlets, JSP, JSF etc..

Need: complex, distributed, internationalized applications, Microservices, cloud, crash prevention, low response time 

Spring is framework comes with a lot of boilerplate code to make developer life easy

SOA - Service-oriented Architecture   
MoM - Message oriented Middle ware  
 Adv: Asynchronous communication, loose coupling between components   
MQ provides buffer if consumer is busy or not connected to network If persistent storage used for MQ then consumer and producer need not be online at the same time   
Routing: Can be done on MoM layer or receiver application.   
Dis Adv: difficult to maintain as extra Broker component   
JMS   
RabitMQ   
AMQP   


### Micros services at Netflix

MS at Netflix [slidehsare link  
 ](https://www.slideshare.net/stonse/pros-and-cons-of-a-microservices-architecture-talk-at-aws-reinvent%20)[https://www.youtube.com/watch?v=CriDUYtfrjs](https://www.youtube.com/watch?v=CriDUYtfrjs)

MQ Intro: [https://docs.oracle.com/cd/E19435-01/819-0069/intro.html](https://docs.oracle.com/cd/E19435-01/819-0069/intro.html)   
RabitMQ Intro - [https://google-ukdev.blogspot.com/2008/09/rabbitmq-tech-talk-at-google-london.html](https://google-ukdev.blogspot.com/2008/09/rabbitmq-tech-talk-at-google-london.html) REST vs MQ: [https://stackoverflow.com/questions/19246704/restful-v-s-mq-differences-and-other-key-features-apart-from-guaranteed-deliver](https://stackoverflow.com/questions/19246704/restful-v-s-mq-differences-and-other-key-features-apart-from-guaranteed-deliver)   
AMQP or HTTP: [https://stackoverflow.com/questions/16838416/service-oriented-architecture-amqp-or-http](https://stackoverflow.com/questions/16838416/service-oriented-architecture-amqp-or-http)   
Java EE: [https://app.pluralsight.com/library/courses/java-ee-getting-started/table-of-contents](https://app.pluralsight.com/library/courses/java-ee-getting-started/table-of-contents)   
MQ: [https://app.pluralsight.com/library/courses/asynchronous-messaging-rabbitmq-easynetq/table-of-contents](https://app.pluralsight.com/library/courses/asynchronous-messaging-rabbitmq-easynetq/table-of-contents)

### Java EE

Build Tools: Apache Ant \(old\), Ivy, Maven \(heavily used\) , Gradle \(latest\)  
Maven - XML based Build Automation tool \(compile, package, clean, dependencies\), Open source, describes how to use program, and dependencies, config file: pom.xml  
Equivalent in .NET is MSBuild/Nuget  
Application Server: Middle ware to provide EE features like for data access, Http access, monitoring etc.. Options: Glassfish, Apache TomEE, Payara Jboss, WildFly  
Tomcat simple HTTP server only \(not full stack EE server\)  
Jboss is like Redhat \(production version\), WildFly is like Fedora \(developer version\)

**Open source Database**:   
MySQL, MariaDB, Derby, SQLite, PostgreSQL, H2  
**H2 Database** - used for development purpose: very fast, single jar file \(smaller footprint\), in-memory embedded mode. Maven used to configure H2 as dependency  


Test Framework: JUnit \(Unit Test\), Arquillian \(Integration test\)  


Java EE development Setup

Install JDK, 

Install Maven 

Install WildFly 17 final \(Eclipse doesn’t support 18 yet\)

Install Eclipse EE edition

Configure Jboss in Eclipse \(to invoke WildFly directly from Eclipse\) 

Configure H2 and JUnit frameworks as dependencies in Maven pom.xml file  


WildFly =  run standalone to start App server, run Adduser once to setup admin user

 start "WildFly" standalone.bat -Djboss.socket.binding.port-offset=100

Check Installation:  java -version, mvn -version,   


JDBC = Low level standard for accessing Database directly using SQL Type statements.

Equivalent in .NET is Entity ODBC/ADO.NET  


JPA = Java Persistence API, specification only \(Hibernate is one of the implementation\) high level abstraction \(with Object Relational Mappings\) to access DB. Easy to use and map DB entries to Java objects than legacy JDBC. 

Equivalent in .NET is Entity framework. 

* Maps objects to relational DB
* Entity Manager
* Entity \(similar to objects but live persistently in DB\)
* CRUD operations
* Query Language JPQL

### Spring boot

#### Links:

Spring Boot ref and API docs: [https://spring.io/projects/spring-boot\#learn](https://spring.io/projects/spring-boot#learn)

Spring Boot Sample projects:  [https://github.com/spring-projects/spring-boot](https://github.com/spring-projects/spring-boot)

Spring boot basics: [https://www.tutorialspoint.com/spring\_boot/index.htm](https://www.tutorialspoint.com/spring_boot/index.htm)

Spring Boot microservices example doc: [https://github.com/OmarElGabry/microservices-spring-boot](https://github.com/OmarElGabry/microservices-spring-boot) 

Spring Boot microservices example code: [https://github.com/OmarElGabry/microservices-spring-boot](https://github.com/OmarElGabry/microservices-spring-boot)

PluralSight Course:  [https://app.pluralsight.com/library/courses/building-first-app-with-spring-boot-angularjs](https://app.pluralsight.com/library/courses/building-first-app-with-spring-boot-angularjs)

Author’s github link: [https://github.com/dlbunker](https://github.com/dlbunker)

Spring boot blogs: [https://piotrminkowski.wordpress.com/](https://piotrminkowski.wordpress.com/) [https://techshard.com/](https://techshard.com/) [https://www.youtube.com/watch?v=fvEWoy1xOvo](https://www.youtube.com/watch?v=fvEWoy1xOvo)  


Quick Guide to Microservices With Spring Boot 2.0, Eureka, and Spring Cloud [https://dzone.com/articles/quick-guide-to-microservices-with-spring-boot-20-e](https://dzone.com/articles/quick-guide-to-microservices-with-spring-boot-20-e)

MicroServices using Spring Boot & Spring Cloud [https://sivalabs.in/2018/03/microservices-part-2-configuration-management-spring-cloud-config-vault/](https://sivalabs.in/2018/03/microservices-part-2-configuration-management-spring-cloud-config-vault/)

Martin flower article: [https://martinfowler.com/articles/microservices.html](https://martinfowler.com/articles/microservices.html)  


#### Spring Boot Basics

Spring = Java framework to develop Enterprise applications

Spring = App server + lots of packages + ORM + logging + MVC 

Spring Boot = Spring + Boot strapping \(add project setup is done like Asp.net MVC App\)

Main Method = @SpringBootApplication annotation from the main class

run\(\) is invoked form inside main\(\) method with main class

Controller:

1\) @RestController on top of the class

 2\) @RequestController on top of URI method \(or class\)

 3\) @GetMapping for get actions like get,  post 

 4\) @PostMapping for post actions

Create JAR: mvn clean install

Clean only: mvn clean

Run App: Java -jar  &lt;JAR\_FILE&gt;

Ex: mvn clean install &&  java -jar ./target/bikedemo-0.0.1-SNAPSHOT.jar

Create WAR package:

1. Update pom.xml with “packaging” attribute
2. Derive main class from SpringBootServletInitializer and override configure\(\) method
3. Run mvn package command

Project structure:

─ src

│   ├── main

│   │ ├── java.com.example.bikedemo

│   │ │               ├── BikedemoApplication.java

│   │ │               ├── controllers

│   │ │               │ └── BikeController.java

│   │ │               ├── models

│   │ │               │ └── Bike.java

│   │ │               └── repositories

│   │ │                   └── BikeRepository.java

│   │ └── resources

│   │     ├── application.properties

│   │     ├── static

│   │     └── templates

│   └── test

│       └── java.com.example.bikedemo

│                       └── BikedemoApplicationTests.java  


Add DB support: Update pom.xml for with 

Spring-boot-starter-data-jpa \(for JPA layer\), sqlite-jdbc \(JDBC driver\),  sqlite-dialect \(Actual DB\)

Pom.xml: \(similar to csproj and sln file in .NET world\)

Contents: Project info, Java version to use \(ex: 1.8\), base spring boot version \(libs\) to use \(ex: 2.2\), spring boot libs, web app libs, build plugin for maveen-springboot build, libs for database access \(jpa+jdbc+db\) libs   


resources/application.properties - \(similar to app.config in .NET world\)

 db connections, db access patterns and other info   
  


### Angular Client Application

#### Links

Ng build \(prod build\) vs ng serve \(development only\)

[https://stackoverflow.com/questions/47150724/what-is-difference-between-ng-build-and-ng-serve](https://stackoverflow.com/questions/47150724/what-is-difference-between-ng-build-and-ng-serve)  
  


[http://localhost:4200/admin](http://localhost:4200/admin) \(List of all bike users\)

[http://localhost:4200](http://localhost:4200/admin) \(To Add new bike user\)

[http://localhost:4200](http://localhost:4200/admin)/server/api/v1/bikes \(Initial implementation without bootstrap and css\)  


Install the following: \(default angular server port 4200\)

sudo pm install node sudo npm install yarn sudo npm install nvm sudo npm install -g @angular/cli

Check version

Node --version npm --version ng --version

New Angular Project:

ng new bikedemo-ui -routing \# New project

npm start \(or ng serve\) \# Start angular

ng serve --proxy-config proxy.conf.json \# if proxy config used

ng g service services/bike \# Add a new service

ng g component components/admin \# Create a Admin component

npm install --save rxjs-compat \# for rxjs/Observable  


npm install bootstrap@ --save \# Bootstrapping the UI

npm install @angular-devkit/core --save \# Bootstrapping style helper  


rm -rf node\_modules && npm install \# Clean Install node modules   


For production build

npm install express-http-proxy --save \# proxy  \(similar to proxy-config.json\)

npm install cors --save \# Enable CORS

npm install port --save \# To use 

ng build --prod=true \# production build \(Creates ./dist for prod distribution\)

node server.js \# start node server

ng serve \# to test changes on local server \(no ./dist directory\)

Create a proxy \(DEV builds only\)  to avoid CORS as Angular and Spring Boot Application runs in different domains

Ex: Create new proxy-config.json file and update package.json

/server": { "target": "[http://localhost:8080](http://localhost:8080)", ..}

Proxy forward: localhost:4200/server/ =&gt;  localhost:4200/localhost:8080

Here /server redirects to Spring boot server at localhost:8080 and redirects the output

Ex: /server/api/v1/bikes =&gt; localhost:8080/api/v1/bikes  


