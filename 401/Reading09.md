
## The HTTP Request Lifecycle

### Step 1: Local Processing : 
- your browser extracts: 
1.protocol (HTTP)
2. host (www.example.com)
3. optional port number, resource path, and query strings that are specified in the form.

### Step 2: Resolve an IP
- Now the browser has the intended hostname for the request. Then the browser will then look through its own cache of recently requested URLs, the operating system’s cache of recent queries, your router’s cache, and your DNS cache, looking for the IP. 
- If an address for the given domain cannot be resolved, the server responds with a failure and your browser returns an error.
- We will assume the request is successful though. Now the requesting client now has a target IP.

### Step 3: Establish a TCP Connection
- Now that the client has an IP address, it can send an HTTP5 request.
- since the request is sent over TCP6, which is a transport layer protocol like UDP, the client must open a TCP connection. One of the key differences between TCP and UDP is that TCP ensures delivery and ordered data transmission.

### Step 4: Send an HTTP Request
**Because the client has an IP address and a TCP connection, it can send an HTTP request.**
- The request is made up of:
1. Request line: The "request line" is simply a line that indicates the HTTP method, the resource being requested, and the protocol version.
2. Header: The header of the request is made up of pairs in the form name:value <CR><LF>. 
3.  Body: The body content of an HTTP request is completely optional, but often contains something like form data or JSON.
 request header, and a body. 

- **Once the server receives the request, processes it, and finds the resource being requested, it generates an HTTP response. An HTTP response has a similar structure to an HTTP request, containing a "status line", response header fields, and an optional body.**

### Step 5: Tearing Down and Cleaning Up
- Once the response has been fully delivered, your browser begins processing what it has received. If it is an image, data, or other media file that is being consumed by some application inside the browser, a variety of things can happen.


## Way of performing HTTP requests

1. by using the built-in Java class HttpUrlConnection, you can perform HTTP requests in Java.

2. The HttpUrlConnection class allows us to perform basic HTTP requests without the use of any additional libraries. All the classes that we need are part of the java.net package.
- Note: The HttpUrlConnection class is used for all types of requests by setting the requestMethod attribute to one of the values: GET, POST, HEAD, OPTIONS, PUT, DELETE, TRACE.

3. We can create an HttpUrlConnection instance using the openConnection() method of the URL class.

4. To add parameters to a request, we have to set the doOutput property to true, then write a String of the form param1=value¶m2=value to the OutputStream of the HttpUrlConnection instance.

5. Adding headers to a request can be achieved by using the setRequestProperty() method.

6. setting the connect and read timeouts.

7. - First, to read the cookies from a response.
- Next, we will add the cookies to the cookie store.
- Finally, to add the cookies to the request.

8. We can enable or disable automatically following redirects for a specific connection by using the setInstanceFollowRedirects() method with true or false parameter.

9. Reading the Response.

10. Reading the Response on Failed Requests.

11. Building the Full Response.

### Resources
- https://dev.to/dangolant/things-i-brushed-up-on-this-week-the-http-request-lifecycle-
- https://www.baeldung.com/java-http-request
