### 1. What is OAuth?
- an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial (security technology), related, single logon credential. 
-  OAuth is for machines logging into machines on behalf of humans.

### 2. Give an example of what using OAuth would look like.
- when you go to log onto a website and it offers one or more opportunities to log on using another website’s/service’s logon. 

### 3. How does OAuth work? What are the steps that it takes to authenticate the user?
1. The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
2. The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
3. The first site gives this token and secret to the initiating user’s client software.
4. The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
5. If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
6. The user approves (or their software silently approves) a particular transaction type at the first website.
7. The user is given an approved access token (notice it’s no longer a request token).
8. The user gives the approved access token to the first website.
9. The first website gives the access token to the second website as proof of authentication on behalf of the user.
10. The second website lets the first website access their site on behalf of the user.
11. The user sees a successfully completed transaction occurring.

### 4. What is OpenID?
- It is a (security technology) for humans logging into machines.
- It is an identity layer built on top of the OAuth 2.0 framework. It allows third-party applications to verify the identity of the end-user and to obtain basic user profile information. 

=====================================

### 1. What is the difference between authorization and authentication?
-  authentication is the process of verifying who a user is, while authorization is the process of verifying what they have access to.
### 2. What is Authorization Code Flow?
- It is used to obtain both access tokens and refresh tokens and is optimized for confidential clients.
- 
### 3. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?
- During authentication, mobile and native applications can use the Authorization Code Flow, but they require additional security. 
To mitigate these, OAuth 2.0 provides a version of the Authorization Code Flow which makes use of a Proof Key for Code Exchange (PKCE).

### 4. What is Implicit Flow with Form Post?
- Implicit Flow with Form Post flow uses OIDC to implement web sign-in . that is very similar to the way SAML and WS-Federation operates. The web app requests and obtains tokens through the front channel, without the need for secrets or extra backend calls. With this method, you don’t need to obtain, maintain, use, and protect a secret in your application.

### 5. What is Client Credentials Flow?
- The client can request an access token using only its client credentials when the client is requesting access to the protected resources under its control, or those of another resource owner that have been previously arranged with the authorization server.

### 6. What is Device Authorization Flow?
- The device asks the user to go to a link on their computer or smartphone and authorize the device, in which they pass along their Client ID to initiate the authorization process and get a token.

### 7. What is Resource Owner Password Flow?
- (A)  The resource owner provides the client with its username and password.

- (B)  The client requests an access token from the authorization server's token endpoint by including the credentials received from the resource owner.  When making the request, the client authenticates with the authorization server.

- (C)  The authorization server authenticates the client and validates  the resource owner credentials, and if valid, issues an access token.

### Resourses:
1. https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html
2. https://auth0.com/docs/flows

