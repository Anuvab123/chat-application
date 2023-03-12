Technology Stack
-
The following technologies and frameworks were used in this project:
Java 8,

Spring Boot,

Spring WebSockets

Mysql,

Swagger

Features
-
This Chat Application provides the following features:

1. ser registration and authentication.
2. Real-time chat messaging between registered users.
3. User profile management

Data Flow
-
1. The data flow in the Chat Application is as follows:

2. User opens the Chat Application in a web browser.

3. User registers or logs in with their email and password. The credentials are validated by the server using Spring Security.

4. Once authenticated, the user is redirected to the chat page. The server sends a list of online users to the client using WebSockets.

5. User selects a user from the list of online users to chat with. The client sends a WebSocket message to the server requesting a new chat session.

6. The server creates a new chat session for the two users and sends the session ID to both clients using WebSockets.

7. The clients use the session ID to send and receive chat messages in real-time using WebSockets.
8. When the user logs out or closes the browser window, the client sends a WebSocket message to the server to notify it of the user's status change. The server removes the user from the list of online users.


Conclusion
-
The Chat Application uses Spring WebSockets to enable real-time communication between clients. The server handles user authentication, creates chat sessions, and sends and receives chat messages using WebSockets. This data flow enables users to communicate in real-time and provides a seamless user experience.