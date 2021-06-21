## Status Codes Based On REST Methods

### In your own words, describe what each group of status code represents:
- 100’s = telling the client that its request will fail before they start sending the body.
- 200’s = telling the client that its request was accepted.
- 300’s = telling the client that the resource they are requesting isn’t available.
- 400’s =  invalid requests a client sent to a server.
- 500’s = unreachable servers.

### What is a status code 202?
- Accepted , Often used for asynchronous processing. This code tells the client that the request was valid, but its processing will finish sometime in the future.

### What is a status code 308?
- Permanent Redirect - This tells the client to use another URL to access the resource and not use the current URL anymore.

### What code would you use if an update didn’t return data to a client?
- 204 (No Content) 

### What code would you use if a resource used to exist but no longer does?
- 414 (Request-URI Too Long)

### What is the ‘Forbidden’ status code?
- 403

## Video

### Why do we need to pull our MongoDB database string out of our server and put it into our .env?
- To deploy our application.

### What is middleware?
- Code that runs once the server got the request but before passed to our routes.

### What does app.use(express.json()) do?
- Make our server accept json as a body inside a post element.

### What does the /:id mean in a route?
- Meaning that it's a parameter and use to get all parameters passed after the slash.

### What is the difference beween PUT and PATCH?
- PUT : update all info 
- PATCH : update only specific item

### How do you make a defalut value in a schema?
- By writing the word `default` .

### What does a 500 error status code mean?
- Server error

### What is the difference between a status 200 and a status 201?
- 200: that the request was received and understood and is being processed.
- 201: indicates that a request was successful and as a result, a resource has been created (for example a new page).

### Resources:
* https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/
* https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw