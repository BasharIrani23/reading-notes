# Web Sockets
### 1- What is a Web Socket?
WebSocket is a computer communications protocol, providing full-duplex communication channels over a single TCP connection.
### 2- Describe the Web Socket request/response handshake and what happens once the connection is established.
To establish a WebSocket connection, the client sends a WebSocket handshake request, for which the server returns a WebSocket handshake response, as shown in the example below.[38]
The handshake starts with an HTTP request/response, allowing servers to handle HTTP connections as well as WebSocket connections on the same port. Once the connection is established, communication switches to a bidirectional binary protocol which does not conform to the HTTP protocol.

### 3- Web Sockets provide a standardized way for the server to send content to a client without first receiving a ____ from that client.
 without first receiving a *request* from that client.
 
 ***
 # Socket.io Tutorial
### 1-What does the event handler *io.on()* do?
It is used to listen for incoming events on the server side.
### 2 -Describe some possible proof of life or proof that the code works as expected
- Create and run test cases covering different scenarios.
- Implement unit tests to validate individual components.
- Perform integration testing to ensure proper collaboration.
- Conduct code reviews for feedback and error detection.
- Engage users in user acceptance testing.
- Implement logging and monitoring for error tracking.
- Set up a CI/CD pipeline for automated testing and deployment.
### 3- What does socket.emit() do?
emit() to send a message to all the connected clients.

*** 
# Socket.io vs Web Sockets

### 1-What is the difference between WebSocket and Socket.IO? (think Git and GitHub, or OAuth and Auth0).

WebSocket is a lower-level protocol that facilitates real-time bidirectional communication between a client and a server. It provides a persistent connection and efficient data transmission.

On the other hand, Socket.IO is a higher-level library that abstracts WebSocket and adds extra functionality, fallback mechanisms, and improved ease of use for real-time applications. It builds upon WebSocket to offer a more comprehensive and flexible solution for real-time communication.

In summary, WebSocket serves as the underlying protocol for real-time communication, while Socket.IO is a library that enhances WebSocket by providing additional features, fallback support, and improved developer experience for building real-time applications.

### 2- When would you use Socket.IO?
- Real-time Applications
- Cross-Browser and Cross-Platform Compatibility
- Automatic Reconnection
- Room-Based Communication
- Event-Based Communication
 ### 3-When would you use WebSockets?
- Real-time web applications that require instant and bidirectional communication.
- Implementing push notification systems for immediate delivery of updates to clients.
- Streaming data applications such as stock tickers or live sports scores.
- Building chat applications for instant messaging.
- Multiplayer online games for real-time interaction among players.
- Live streaming and broadcasting applications.
