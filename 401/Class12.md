# Readings: Socket.io

# Notes and summary
## what is a WebSocket?

- It is a computer communications protocol, providing full-duplex communication channels over a single TCP connection.
<br/>
<br/>

- The Transmission Control Protocol (TCP) is one of the main protocols of the Internet protocol suite. It originated in the initial network implementation in which it complemented the Internet Protocol (IP). Therefore, the entire suite is commonly referred to as TCP/IP. TCP provides reliable, ordered, and error-checked delivery of a stream of octets (bytes) between applications running on hosts communicating via an IP network.

<br/>
<br/>

## What is Socket.IO?
-It is a JavaScript library for real-time web applications. It enables real-time, bi-directional communication between web clients and servers. 
<br/>
<br/>

## Socket.IO have two parts, mention them?
- It has two parts: a client-side library that runs in the browser, and a server-side library for node.js. Both components have an identical API.
<br/>
<br/>



## Key features of WebSocket:
1. WebSocket helps in real-time communication between the Client and the webserver.
2. This protocol helps in transforming to cross-platform in a real-time world between the server and the client.
3. This also enables the business worldwide for a real-time web application to enhance and increase the feasibility.
4. The major advantage it stands over an HTTP connection that it provides full-duplex communication.
<br/>
<br/>


## WebSocket protocol schema:
![schema](../images/WebSocket-protocol-schema.png)

<br/>
<br/>


## Why do we need WebSocket?
1. It provides full-duplex communication, which helps in persisting the connection established between the Client and the Web Server.
2. It also lives up to the standards and provides the accuracy and efficiency stream events to and from with negligible latency.
3. WebSocket removes the overhead and reduce complexity.
4. It makes real-time communication effortless and efficient.
<br/>
<br/>


## Review, Research, and Discussion


1. What is the benefit of transforming data into packets?
- The benefit of transforming data into packets is to be able to transfer them individually to reach their destination. Upon reaching their destination, the destination recompiles the data passed thru the packet to adhere to the protocols of whichever TCP/UDP level they are at in the process.


2. UDP is often refereed to as a connectionless protocol. Why is this?
- Because No connection needs to be established between the source and destination before you transmit data.

3. Can a socket server application have multiple socket connections?
- 65,536 sockets

4. Can a socket connection application be connected to multiple socket servers?
- No.
5. Can an application be both a socket server and a socket connection?
- Yes.

<br/>
<br/>


## Document the following Vocabulary Terms

- Observer Pattern: a behavioral design pattern that lets you define a subscription mechanism to notify multiple objects about any events that happen to the object they’re observing.This is what allows us to emit into a “hub” and have whichever applications that are connected to that “hub” be able to listen for what is emitted and then act accordingly.

- Listener: waits for a predefined (or just created/emitted) event to occur before running code.

- Event Handler:is the function that is run which is dependent upon the event listener having happened

- Event Driven Programming: is a programming paradigm in which the flow of the program is determined by events such as user actions, sensor outputs, or message passing from other programs or threads.

- Event Loop:has one simple job — to monitor the Call Stack and the Callback Queue. If the Call Stack is empty, the Event Loop will take the first event from the queue and will push it to the Call Stack, which effectively runs it. Such an iteration is called a tick in the Event Loop.

- Event Queue: a list of messages to be processed. Each message has an associated function which gets called in order to handle the message. At some point during the event loop, the runtime starts handling the messages on the queue, starting with the oldest one.


- Call Stack:  is a stack data structure that stores information about the active subroutines of a computer program.

- Emit/Raise/Trigger:these words are synonymous and refer to when an event is being created using the emit() method.

- Subscribe:is an object that represents a disposable resource, usually the execution of an Observable.

- database:- is a data structure that stores organized information. Most databases contain multiple tables, which may each include several different fields. For example, a company database may include tables for products, employees, and financial records.

 <br/>
 <br/>

## Preview

1. Which 3 things had you heard about previously and now have better clarity on?
- event loop.

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
- How to connect everything.
3. What are you most excited about trying to implement or see how it works?
- today's lab :P.


<br/>



## References: 

[1. Socket.io Documentation](https://socket.io/docs/)
[2. Socket.io Server API](https://socket.io/docs/server-api)
[3. Socket.io Client API](https://socket.io/docs/client-api)
[4. Socket Testing Tool](https://amritb.github.io/socketio-client-tool/)