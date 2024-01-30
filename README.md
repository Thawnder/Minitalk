# minitalk

**minitalk** is a project at 42 School that involves creating a simple client-server communication program using signals. It consists of two programs: a server and a client. The client sends messages to the server, and the server receives and displays them.

## Features
- Simple client-server communication using signals.
- Lightweight and efficient implementation.
- Supports bidirectional communication between client and server.
- Supports Unicode characters. (bonus)

## Usage
1. Clone the repository:
   <pre>
   git clone https://github.com/Thawnder/minitalk.git
   </pre>
2. Compile the server and client programs:
   <pre>
   make
   </pre>
3. Run the server:
   <pre>
   ./server
   </pre>
4. In another terminal window, run the client with the server's process ID and the message to send:
   <pre>
   ./client server_pid "Hello, server!"
   </pre>
   Replace `server_pid` with the process ID of the server obtained in step 3.

## Example
<pre>
# Terminal 1 (Server)
$ ./server
Server PID: 12345
Received message: Hello, client!

# Terminal 2 (Client)
$ ./client 12345 "Hello, server!"
Message sent successfully!
</pre>
