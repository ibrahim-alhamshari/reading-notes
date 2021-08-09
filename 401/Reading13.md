### Integration Testing in Spring
- verifying the end-to-end behavior of a system.
- Several Maven dependencies are required for running the integration tests .

### Spring MVC Test Configuration
- Enable Spring in Tests with JUnit 5
* JUnit 5 defines an extension interface through which classes can integrate with the JUnit test.
- You can enable this extension by adding the `@ExtendWith` annotation to your test classes and specifying the extension class to load.
-  `@ContextConfiguration` annotation to load the context configuration and bootstrap the context that your test will use.

### Writing Integration Tests
Example:
`@Test`
`public void givenHomePageURI_whenMockMVC_thenReturnsIndexJSPViewName() {`
   ` this.mockMvc.perform(get("/homePage")).andDo(print())`
      `.andExpect(view().name("index"));`
`}`

### Many-to-Many Relationship
- It is defined using @ManyToMany annotation, to which we can add @RestResource.

- To create a many-to-many relationship, add a new model class that will have a many-to-many relationship with the Book entity.

- create a repository interface to manage the Author entity.
 Ex: `public interface AuthorRepository extends CrudRepository<Author, Long> { }`

### Resources
- https://www.baeldung.com/spring-data-rest-relationships
- https://www.baeldung.com/integration-testing-in-spring