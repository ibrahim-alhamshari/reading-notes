## Spring Boot and OAuth2
- building a sample app doing various things with "social login" using OAuth 2.0 and Spring Boot. The samples are all single-page apps using Spring Boot and Spring Security on the back end. It starts with a simple, single-provider single-sign on.

> There are several samples building on each other, adding new features at each step, they all come up with a home page on http://localhost:8080, It requires at least a GitHub and Google account if you want to log :

1. simple: It's unconditional login in the home page.
2. click: adds an explicit link that the user has to click to login.
3. logout: adds a logout link as well for authenticated users.
4. two-providers: adds a second login on the home page, and the user can choose one of them.
5. custom-error: adds an error message for unauthenticated users.

- To make the application secure, you can add Spring Security as a dependency. Since you’re wanting to do a "social" login (delegate to GitHub), you should include the Spring Security OAuth 2.0 Client starter.

- Adding the Login Link in the HTML file

<div class="container unauthenticated">
  <div>
    With GitHub: <a href="/oauth2/authorization/github">click here</a>
  </div>
  <div>
    With Google: <a href="/oauth2/authorization/google">click here</a>
  </div>
</div>

- **Adding a Logout Endpoint with**
Spring Security  support a `/logout` endpoint which will do (clear the session and invalidate the cookie).

### Resources
- https://spring.io/guides/tutorials/spring-boot-oauth2/



