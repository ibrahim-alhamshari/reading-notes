## Using `WebSocket` to build an interactive web application

> WebSocket is used to develop two-way communication between server and browser. For example, in a chat application, if a user sends a message to a different user, the application sends that message to the server first and the server informs the application of the second user . If we don’t use WebSocket, the application or the client will have to pull the server data continuously for any new updates.


![WebSocket](https://th.bing.com/th/id/R.0f7207fd6853090a7544aad83c2573ff?rik=j3U6l3bQeVS3HQ&riu=http%3a%2f%2fjavasampleapproach.com%2fwp-content%2fuploads%2f2017%2f06%2fspring-websocket-architecture-new-ws.png&ehk=vWSqCCJaAuWVPH1yMyZn%2bo%2f9TPWZYfj32xCA7EtkpSM%3d&risl=&pid=ImgRaw&r=0)

- To build a server that accepts a message that carries a user’s name. In response, the server will push a greeting into a queue to which the client is subscribed. And to do that you have to:
1. Create a Resource Representation Class
- The service will accept messages that contain a name in a STOMP message whose body is a JSON object. The service will process it by creating a greeting and publishing that greeting on a separate queue to which the client is subscribed. The greeting will also be a JSON object

2. Create a Message-handling Controller
- You need to implement the: `@MessageMapping`

3. Configure Spring for STOMP messaging
4. Create a Browser Client (HTML) that will send messages to and receive messages from the server side.
