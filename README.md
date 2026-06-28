# A Mini Multi Threaded 21CS Chat Room Created in Java

<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/97f29433-7048-493f-9887-3ea6616ce328" />

This project is a Java-based implementation of a multi-threaded chat room. It serves as an educational tool to demonstrate the practical application of **socket programming**, **multi-threading**, and **client-server architecture**.

## Project Overview

Created for the Operating Systems course, this application allows multiple clients to connect to a single server and communicate in real-time. It leverages Java's concurrency mechanisms to handle multiple connections simultaneously without blocking.

## Key Features

- **Real-time Messaging:** Concurrent messaging between multiple connected clients.
- **Multi-threading:** Uses `ExecutorService` for efficient handling of client connections.
- **Dynamic Nicknames:** Support for changing usernames using the `/nick <new_name>` command.
- **Graceful Exit:** Clients can leave the chat room using the `/quit` command, which notifies all other users.
- **Robust Networking:** Built on TCP/IP socket programming.

## Requirements
- **Java Development Kit (JDK) 17** or higher.
- A terminal or Command Prompt (CLI).

## How to Run
To run the project, follow these steps in your Command Prompt/Terminal:

**1. Compile the source code:**
Navigate to the root directory where the `src` folder is located and run:
```
javac src/Server.java src/Client.java
```

**2. Start the Server:**
```
java src.Server
```

**3. Start the Client(s):**
Open a new command prompt window for each client and run:
```
java src.Client
```

## Technical Architecture
The system follows a standard Client-Server model where the Server acts as a central hub, managing threads for each incoming connection to ensure non-blocking communication.

## Limitations & Future Directions
As this was an educational project, there are known limitations that could be addressed in future iterations:

- **Security:** Lack of encryption or user authentication.
- **Persistence:** No database integration; messages are lost if the server stops.
- **Interface:** Current implementation uses a CLI; a GUI (JavaFX/Swing) could be implemented for a more user-friendly experience.
