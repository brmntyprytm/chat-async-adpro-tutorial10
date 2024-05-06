# Tutorial 10 - Async Programming

### 2.1 Original code of broadcast chat.

![imag1](imag/image1.png)
![imag2](imag/image2.png)
The client sends a message to the server, and the server receives it and echoes it back to the client.
This exchange demonstrates bidirectional communication between the server and client over the established connection.
Both the server and client seem to be properly configured to send and receive messages.

### 2.2 Modifying the websocket port

This modification establishes a chat system using WebSockets. The server, running on port 8080, listens for messages from clients. When a client connects, it can send messages to the server, which then broadcasts them to all connected clients, enabling real-time chat. The tokio_websockets crate simplifies the communication process.
