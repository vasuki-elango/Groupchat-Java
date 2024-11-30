# Groupchat-Java

### `System Requirements`
1.	Java Development Kit (JDK): Version 8 or higher.
2.	Command-Line Terminal: Compatible with Windows CMD, Linux Terminal, or macOS Terminal.
3.	Network Connectivity: Users should be on the same network or configured subnet.


### `Technologies and Concepts Used`
1.	Java Networking:
MulticastSocket: For joining a multicast group and sending/receiving messages.
DatagramPacket: To encapsulate data sent or received in the multicast group.
2.	Multithreading:
A dedicated thread reads incoming messages, ensuring the main thread remains responsive for user input.
3.	I/O Streams:
Handles input from the user and processes network communication.
4.	Character Encoding:
Uses UTF-8 to ensure compatibility and proper display of messages across different systems.
5.	Group Communication Protocols:
Configures TimeToLive for controlling the scope of message propagation.

### `Sample Commands `
# Start the Program:
javac GroupChat.java
java GroupChat <multicast-host> <port-number>
Example: java GroupChat 224.0.0.1 5000
# Exit the Chat:
Type Exit in the terminal and press Enter.

### `Strengths of the Project`
1.	Simple and Lightweight: Runs entirely on the command line without additional dependencies.
2.	Real-time Communication: Uses UDP multicast for efficient message broadcasting.
3.	Scalability: Multiple users can join the same multicast group without additional server configuration.
