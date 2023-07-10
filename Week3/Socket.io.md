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

