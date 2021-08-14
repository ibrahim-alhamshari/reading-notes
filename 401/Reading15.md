## Authentication and Access Control
- Application security boils down to two more or less independent problems: **`authentication`** (who are you?) and **`authorization`** (what are you allowed to do?).

### Authentication
The main strategy interface for authentication is `AuthenticationManager`. It has one method and in this method, you can do only one thing of these three things:
1. Return an Authentication (normally with authenticated=true) if it can verify that the input represents a valid principal.

2. Throw an AuthenticationException if it believes that the input represents an invalid principal.

3. Return null if it cannot decide.

### Authorization or Access Control
- Once **`authentication`** is successful, we can move on to **`authorization`**, and the core strategy here is `AccessDecisionManager`. 

>**There are three implementations provided by the framework**
- `AccessDecisionVoter`: considers an Authentication (representing a principal) and a secure Object.
- `ProviderManager` and `AuthenticationProviders` : It represents anything that a user might want to access (a web resource or a method in a Java class are the two most common cases).

### Web Security
- It is based on Servlet `Filters`. A `filter` can also modify the request or the response used in the downstream filters and servlet. 

![Spring Security](https://github.com/spring-guides/top-spring-security-architecture/raw/main/images/filters.png)

- The client sends a request to the application, and the container decides which filters and which servlet apply to it based on the path of the request URI. At most, one servlet can handle a single reques.


### From Spring Auth Cheat Sheet:
- Step 1: set up a user model and repo
- Step 2: create a controller for that model
- Step 3: UserDetailsServiceImpl implements UserDetailsService
- Step 4: ApplicationUser implements UserDetails
- Step 5: WebSecurityConfig extends WebSecurityConfigurerAdapter
- Step 6: registration page
- Step 7: login page

### Resources
- https://spring.io/guides/topicals/spring-security-architecture/
- https://github.com/codefellows/seattle-java-401d2/blob/master/SpringAuthCheatSheet.md