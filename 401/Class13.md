
# Readings: Message Queues


## Review, Research, and Discussion


1. What does it mean that web sockets are bidirectional? Why is this useful?
- This means that sockets can facilitate information flowing into and out of a socket connection between a socket server and client.

<br/>

2. Does socket.io use HTTP? Why?
- Yes, the initial connection setup is done with HTTP.
<br/>


3. What happens when a client emits an event?
- The client emits an event and then the server handles the event using the on method.
<br/>




4. What happens when a server emits an event?
- The server emits an event and then the client that the event was emitted to handles the event.
<br/>



5. what happens if a client “misses” an event?
- it will not run the evet handler.
<br/>



6. How can we mitigate this?
- unheard events should be stored in a queue system on the server that is resumed as a client connects.
<br/>


<br/>
<br/>
<br/>


# Terms"


1. Socket: protocol to open the network connection for the program, allowing data to be read and written over the network.



2. Web Socket:Its a computer communications protocol providing full-duplex communication channels over a single TCP connection.*


3. Socket.io: Its a library that enables real-time, bidirectional and event-based communication between the browser and the server.

4. Client: the entity requesting data in a transaction.

5. Server: It's a computer that serves information to other computers(clients).

6. OSI Model:  a conceptual model that characterises and standardises the communication functions of a telecommunication or computing system without regard to its underlying internal structure and technology.

7. TCP Model: the conceptual model and set of communications protocols used in the Internet and similar computer networks. It is commonly known as TCP/IP because the foundational protocols in the suite are the Transmission Control Protocol and the Internet Protocol.

8. TCP: The Transmission Control Protocol is one of the main protocols of the Internet protocol suite. It originated in the initial network implementation in which it complemented the Internet Protocol.

9. UDP: In computer networking, the User Datagram Protocol is one of the core members of the Internet protocol suite. With UDP, computer applications can send messages, in this case referred to as datagrams, to other hosts on an Internet Protocol network.

10. Packets: a formatted unit of data carried by a packet-switched network. A packet consists of control information and user data; the latter is also known as the payload.

<br/>
<br/>
<br/>


## preview

- Which 3 things had you heard about previously and now have better clarity on? 
- sql.

- Which 3 things are you hoping to learn more about in the upcoming lecture/demo?  
- more sql

- What are you most excited about trying to implement or see how it works? 
- connecting database with socket.io


<br/>
<br/>
<br/>

## References:

1. [Socket.io Chat Example](https://socket.io/get-started/chat/)
2. [Rooms and Namespaces](https://socket.io/docs/rooms-and-namespaces/)
3. [Socket.io Emit Cheatsheet](https://socket.io/docs/emit-cheatsheet/)