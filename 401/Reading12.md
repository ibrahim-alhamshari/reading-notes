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