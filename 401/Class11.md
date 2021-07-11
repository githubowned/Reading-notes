# Readings: Event Driven Applications



## Event Driven Applications
- Event Driven Programming
Event-Driven Programming is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision.

- An event driven programming approach uses events to trigger various functions. An event can be anything, such as typing a key or clicking a mouse button. A call-back function is already registered with the element executes whenever an event is triggered.

- In an event-driven application, there is generally a main loop that listens for events and then triggers a callback function when one of those events is detected. In embedded systems, the same may be achieved using hardware interrupts instead of a constantly running main loop. Event-driven programs can be written in any programming language, although the task is easier in languages that provide high-level abstractions, such as await and closures.

## EventEmitter
Node.js natively provides us with a useful module called EventEmitter that allows us to get started incorporating Event-Driven Programming in our project right away. Of course, creating our own version of EventEmitter wouldn’t be much of a challenge, and in fact there are several modules published on npm such as EventEmitter2 and EventEmitter3 which promise a faster performance than the native EventEmitter.




## Removing Listeners
- There will likely come a time when you want to remove an event listener from an event. This could be for performance reasons (the event is no longer needed) or to avoid memory leaks (if an event listener references an object that is no longer needed, it won’t be able to be garbage-collected. This can lead to a build up of unnecessary objects).


## REVIEW, RESEARCH & DISCUSSION

- Access control is important for site management, in that it gives certain users certain access to certain areas of the site.

- The word press hosted website that my organzation uses is an example of a web application that benefits from access control. Only one person is able to make an post edits to pages, as the admin, and other people are only able to view content or edit but not update.

- A role is used to determine what a user has access and the ability to do within the site.

- Role based access “makes it simple for owners to manage users in groups based on their role or position, rather than assigning permissions to each specific individual. RBAC largely eliminates discretion when providing access to objects” source (Links to an external site.)

- Authorization: authorization typically requires a bearer token of the user. Access to different resources within a site is based on the token that connected a particular user.

- Role Based Access Control: granted permission and access to resources or areas of a site based on attributes associated with a users defined role.

- Capabilities: are what and how the user is able to access or contribute to a site. Example of capabilities could be the ability to edit users, create users or delete users.
<br/>



## Document the following Vocabulary Terms


- Event-Driven Programming in Node.js
Event-Driven Programming is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision.For the most recognizable example of Event-Driven Programming for people at any level of programming skill, we’ll turn to our old friend The Web Browser.

<br/>
- Event-Driven Programming makes use of the following concepts:

- An Event Handler is a callback function that will be called when an event is triggered.
A Main Loop listens for event triggers and calls the associated event handler for that event.
EventEmitter

- Node.js natively provides us with a useful module called EventEmitter that allows us to get started incorporating Event-Driven Programming in our project right away.

```
const EventEmitter = require('events').EventEmitter;
const myEventEmitter = new EventEmitter;
Removing Listeners
```

- There will likely come a time when you want to remove an event listener from an event. This could be for performance reasons (the event is no longer needed) or to avoid memory leaks (if an event listener references an object that is no longer needed, it won’t be able to be garbage-collected. This can lead to a build up of unnecessary objects).

```
const EventEmitter = require('events').EventEmitter;
const chatRoomEvents = new EventEmitter;
```

```
function userJoined(username){
  chatRoomEvents.on('message', function(message){
    document.write(message);
  })
}

chatRoomEvents.on('userJoined', userJoined);
```


## References:
1. [Event Driven Programming](https://alligator.io/nodejs/event-driven-programming/)
2. [Node docs: events](https://nodejs.org/api/events.html)