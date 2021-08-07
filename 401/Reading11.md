### Manual Initialization for the project with Spring MVC

**If you want to initialize the project manually, follow the steps below:**

1. Navigate to [Start_Spring](https://start.spring.io.) This service pulls in all the dependencies you need for an application and does most of the setup for you.

2. Choose either Gradle or Maven and the language you want to use. This guide assumes that you chose Java.

3. Click Dependencies and select Spring Data JPA and then H2 Database.

4. Click Generate.

5. Download the resulting ZIP file, which is an archive of a web application that is configured with your choices.


**The test**
1. Adding the awaitility Dependency: this test require the `awaitility` library.
2. Create a Scheduled Task : The Scheduled annotation defines when a particular method runs.
- EX: `@Scheduled(fixedRate = 5000)`
	`public void reportCurrentTime() {`
		`log.info("The time is now {}", dateFormat.format(new Date()));`
	`}`

**Build an executable JAR**
- You can run the application from the command line with Gradle or Maven. You can also build a single executable JAR file that contains all the necessary dependencies, classes, and resources and run that. 

### Thymeleaf
- It is a popular server-side template engine for Java applications. You can integrate it into a Spring Boot project to develop web applications.

- **In a typical Spring MVC application, @Controller classes are responsible for preparing a model map with data and selecting a view to be rendered, also the model map transform into a Thymeleaf context object.**

- **Spring model attributes are useful for transferring data from Spring controllers to Thymeleaf views. And they are called context variables.**

- **Request parameters: They are passed from the client to server and can be accessed in Thymeleaf views.**

### Resources
- https://spring.io/guides/gs/serving-web-content/
- https://www.thymeleaf.org/doc/articles/springmvcaccessdata.html