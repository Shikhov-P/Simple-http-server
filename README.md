#Simple HTTP server written in Java
##This repos contains a server which can:
* Listen and accept a request from a client
* Respond to a client with the current date and a 200 OK message

##Java classses in use:
* **[java.io.IOException](https://docs.oracle.com/javase/7/docs/api/java/io/IOException.html)** to notify about i/o exceptions
* **[java.net.ServerSocket](https://docs.oracle.com/javase/7/docs/api/java/net/ServerSocket.html)** to implement a socket server that monitors for incoming requests over a network
* **[java.net.Socket](https://docs.oracle.com/javase/7/docs/api/java/net/Socket.html)** to allow using client sockets (an endpoint for communication between two nodes in a network)
* **[java.util.Date](https://docs.oracle.com/javase/7/docs/api/java/sql/Date.html)** to handle date format


`ServerSocket` methods in use:
* accept() (a blocking method that blocks execution until a client connects to the server)

`Socket` methods in use:
* getOutputStream() to allow writing to an output stream;
This method returns an `OutputStream` object to write (output) data into
* write() to write into a client socket

`String` method in use:
* getBytes(charsetName) to encode a string (`httpResponse`) to byte array using a UTF-8 encoding