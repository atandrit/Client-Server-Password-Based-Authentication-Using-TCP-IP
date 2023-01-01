
# Client Server Password Based Authentication Using TCP/IP

This Client-Server program would facilitate a client to register itself via request to the server
and authenticate the user login based on the user identification and password entered at client
side. The server also holds a table that contains all the approved and registered users.
Once connection is established through id and password authentication, user can communicate
through the client with the server.


## Requirement Analysis

Requirement are as follows:
1. Pycharm IDE for Running Client and Server Side Code
2. The client should be starting first.
3. TCP/IP Network design.
4. Run the server first then the client.
5. Free ports
6. Sockets for connecting server and client.
## Algorithm

### Server :
1. Include the necessary header files.
2. Create a socket using socket function with family AF_INET, type as SOCK_STREAM.
3. Bind the local host address to socket using the bind function
4. Listen on the socket for connection request from the client.
5. Accept connection request from the client using accept function.
6. Within an infinite loop, using the recv function receive message from the client and print it on the console.
7. Using hash Table store the user id along with decrypted password.

### Client :
1. Include the necessary header files
2. Create a socket using socket function with family AF_INET, type as SOCK_STREAM.
3. Get the server IP address and port number from the console
4. Request a connection from the server using the connect function
5. Using recv() and send() function , the username and encrypted password is sent from client to server.
## Conclusion

Thus authentication using client server communication was established successfully ,using TCP
model in which user can register on client end using username and password , wherein the
credentials of the user gets stored on server side.
This is the foundation for a highly secured and controlled environment for chat based
communication between more than one registered user.
## Authors

- [@atandrit](https://github.com/atandrit)

