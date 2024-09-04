# 💬 Concurrent TCP Chat

This project involves creating a multi-client chat system using the TCP protocol, where multiple clients can connect to a server and communicate with each other in real-time.

## Goal

Design and implement a simple TCP chat server that allows multiple clients to connect and communicate with each other, demonstrating knowledge of network programming and concurrency.

## Skills

- Consolidate your knowledge of network programming and concurrency.
- Grasp how concurrency aids in solving the issue of blocking I/O.
- Practice packaging software with Maven to ensure a seamless build for both server and client projects.

### Key Points:

- Implement two main components: the **Client** and the **Server**.
- Create any necessary classes for implementing the desired behavior. However, the program should include at least the following functionalities:

  I. **Client Program**
     - The client must connect to the server, set a username upon entry, and be able to send and receive messages.
     - Consider how blocking I/O will be handled and how many threads will be necessary for the client program.

  II. **Server Program**
      - The server must accept multiple client connections concurrently, broadcasting received messages to all connected clients.
      - The server should also support the `/quit` command to allow users to exit the chat.
      - Determine how many threads the server will need to manage simultaneous client communications effectively.

  III. **Commands**
      - Implement essential commands like `/list`, `/whisper`, `/name`, and `/help` to enhance the chat experience.
      - These commands can allow listing connected clients, sending private messages, changing usernames, and displaying available commands.

  IV. **Netcat for Testing**
      - Use Netcat as a server to simulate client-side behavior or as a client to simulate server-side behavior during development.
      - Ensure that the client can connect to a specified IP address and port, and verify the server’s ability to handle multiple connections by simulating several clients.

### Build Instructions

To build the project using Maven, use the `pom.xml` file provided. This file will package both the client and server projects into JAR files. To do so, run this command:

```bash
mvn package
```
This will create two executable JAR files, one for the client and one for the server.

## Requirements

- Java Development Kit (JDK) 17 or above.
- Apache Maven.
- A Java IDE like IntelliJ IDEA, or any other of your choice.

## Installation

Clone the repository and navigate to the folder.

```bash
git clone <repository-url>
cd <repository-folder>
```

## Usage

### Running the Server

To run the server program:

```bash
java -jar target/server.jar
```

To run the clent program:

```bash
java -jar target/client.jar
```

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## Suggested Future Improvements

- Implement additional commands for more functionality, such as sending direct messages or changing chat rooms.
- Enhance the user interface for the client to make it more user-friendly.
- Add a graphical user interface (GUI) to improve the client experience.

## Contributors

-  Daniel Magalhães - [@Housecold](https://github.com/Housecold)
-  Omid Pournejati - [@TheOmidious](https://github.com/TheOmidious)
