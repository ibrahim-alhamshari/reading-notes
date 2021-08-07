### @RequestMapping
- It is one of the most common annotation used in Spring Web applications. This annotation maps HTTP requests to handler methods of MVC and REST controllers.

1. @RequestMapping — by Path
2. RequestMapping and HTTP Headers
3. RequestMapping With Path Variables
4. RequestMapping With Request Parameters
5. RequestMapping Corner Cases
6. New Request Mapping Shortcuts: These new annotations can improve the readability and reduce the verbosity of the code.Thay are:
- @GetMapping
- @PostMapping
- @PutMapping
- @DeleteMapping
- @PatchMapping


### Manual Initialization (optional)
**If you want to initialize the project manually rather than use the links shown earlier, follow the steps given below:**

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


### Spring Data Repositories: 
- I will explain the difference between the three repositories, which are:
1. CrudRepository provides CRUD functions
2. PagingAndSortingRepository provides methods to do pagination and sort records
3. JpaRepository provides JPA related methods such as flushing the persistence context and delete records in a batch

> In CrudRepository functionality we have:
- save(…) – save an Iterable of entities.
- findOne(…) – get a single entity based on passed primary key value
- findAll() – get an Iterable of all available entities in database
- count() – return the count of total entities in a table
- delete(…) – delete an entity.
- exists(…) – verify if an entity exists.

> PagingAndSortingRepository extends CrudRepository:
When we create a Pageable object we've to specify at least:
1.Page size
2. Current page number
3. Sorting

> JpaRepository have these methods:
- findAll() – get a List of all available entities in database
- save(…) – save an Iterable of entities. Here, we can pass multiple objects to save them in a batch
- flush() – flush all pending task to the database
- saveAndFlush(…) – save the entity and flush changes immediately
- deleteInBatch(…) – delete an Iterable of entities. Here, we can pass multiple objects to delete them in a batch.

### Resources
- http://www.baeldung.com/spring-requestmapping
- https://spring.io/guides/gs/accessing-data-jpa/
- https://www.baeldung.com/spring-data-repositories