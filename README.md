MULTITHREADED CHAT APPLICATION

Company: CodTech IT Solutions Pvt. Ltd

Name: Mansi Pokhriyal

Intern ID: CT08DA549

Domain: Java Programming

Duration: 8 Weeks

Mentor: Neela Santosh

Project Title: Multithreaded Chat Application – Java Client-Server System
Project Overview
During my internship at CodTech IT Solutions, I worked on a project titled "Multithreaded Chat Application", which involved creating a text-based communication system that supports real-time messaging between multiple users. This system was built using Java and follows a classic client-server architecture where several clients can connect to a centralized server using TCP/IP sockets.

The project’s main focus was on implementing multithreading and managing simultaneous client interactions efficiently. Each client connection runs on its own thread, allowing users to exchange messages in real-time without delays or interruptions.

Technologies and Tools Used
Language: Java

Key Java APIs:

Socket, ServerSocket – To manage TCP connections.

DataInputStream, DataOutputStream – For reading and writing messages in UTF format.

Thread, Runnable – For handling each client in a separate thread.

Vector – Used to store active client threads safely in a multi-threaded environment.

Development Environment:

Editor: Visual Studio Code with Java extensions

Testing Tools: Used terminal to launch server, and separate command prompts for each client during testing.

Application Architecture
🔹 Server-Side (ChatServer.java)
Runs on port 1234 and waits for incoming client connections using a ServerSocket.

Upon a new client connection:

Initializes input and output streams.

Launches a new ClientHandler thread for managing communication with that client.

Adds the client to a Vector for tracking all active users.

Any message received from a client is broadcast to all other connected clients.

If a client sends the message "exit", their connection is closed cleanly.

🔹 Client-Side (ChatClient.java)
Connects to the server at localhost:1234.

Starts two separate threads:

Send Thread: Captures user input from the console and sends it to the server.

Receive Thread: Continuously listens for messages from the server and displays them.

The client application terminates gracefully when the user types "exit".

Real-World Relevance
This project simulates the foundational functionality found in many real-time communication systems. Examples include:

Instant Messaging Apps: Similar architecture is used in apps like Slack, Discord, or WhatsApp.

Customer Support Systems: Enables agents to chat live with customers.

Online Multiplayer Games: Manages player communications and updates in real-time.

Collaborative Workspaces: Applications like shared editors or whiteboards rely on similar real-time message handling.

Through this task, I gained hands-on exposure to concurrent programming, network communication, and scalable software design — skills essential in enterprise software development.

Conclusion
The Multithreaded Chat Application project was a successful implementation of Java networking and multithreading concepts. It demonstrated how to design a responsive and scalable server capable of handling multiple client interactions simultaneously. This assignment helped deepen my understanding of real-time systems and the underlying technologies that power many modern communication platforms.


#OUTPUT:-

![Image](https://github.com/user-attachments/assets/30acb106-bdd6-498a-9178-385bac7b5663)
