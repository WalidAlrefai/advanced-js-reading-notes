# class 12

# Socket.io

Socket.IO is a library that enables low-latency, bidirectional and event-based communication between a client and a server.

![](./bidirectional-communication2.png)

### Real-time Applications

A real-time application (RTA) is an application that functions within a period that the user senses as immediate or current.

Some examples of real-time applications are :

- Instant messengers − Chat apps like Whatsapp, Facebook Messenger, etc. You need not refresh your app/website to receive new messages.

- Push Notifications − When someone tags you in a picture on Facebook, you receive a notification instantly.

- Collaboration Applications − Apps like google docs, which allow multiple people to update same documents simultaneously and apply changes to all people's instances.

- Online Gaming − Games like Counter Strike, Call of Duty, etc., are also some examples of real-time applications.

## Why Socket.IO?

Writing a real-time application with popular web applications stacks like LAMP (PHP) has traditionally been very hard. It involves polling the server for changes, keeping track of timestamps, and it is a lot slower than it should be.

Sockets have traditionally been the solution around which most real-time systems are architected, providing a bi-directional communication channel between a client and a server. This means that the server can push messages to clients. Whenever an event occurs, the idea is that the server will get it and push it to the concerned connected clients.

Socket.IO is quite popular, it is used by **Microsoft Office**, **Yammer**, **Zendesk**, **Trello**,. and **numerous** other organizations to build robust real-time systems. It one of the most powerful **JavaScript** **frameworks** on **GitHub**, and most depended-upon NPM (Node Package Manager) module. Socket.IO also has a huge community, which means finding help is quite easy.

**WebSocket** is a computer communications protocol, providing full-duplex communication channels over a single TCP connection.

**WebSocket** is distinct from HTTP. Both protocols are located at layer 7 in the OSI model and depend on TCP at layer 4. Although they are different, RFC 6455 states that WebSocket "is designed to work over HTTP ports 443 and 80 as well as to support HTTP proxies and intermediaries", thus making it compatible with HTTP. To achieve compatibility, the WebSocket handshake uses the HTTP Upgrade header to change from the HTTP protocol to the WebSocket protocol.

## Difference Between WebSocket and Socket.io

WebSocket is the communication Protocol that provides bidirectional communication between the Client and the Server over a TCP connection; WebSocket remains open all the time, so they allow real-time data transfer. When clients trigger the request to the server, it does not close the connection on receiving the response; it rather persists and waits for the Client or server to terminate the request.

Socket.IO is a library that enables real-time and full-duplex communication between the Client and the Web servers. It uses the WebSocket protocol to provide the interface. Generally, it is divided into two parts; both WebSocket vs Socket.io are event-driven libraries.

### Key features of Socket.IO

- It helps in broadcasting to multiple sockets at a time and handles the connection transparently.
- It works on all platform, server or device, ensuring equality, reliability, and speed.
- It automatically upgrades the requirement to WebSocket if needed.
- It is a custom real-time transport protocol implementation on top of other protocols.
- It requires both libraries to be used Client side as well as a server-side library.
- IO works on work-based events. there are some reserved events that can be accessed using the Socket on the  server side like Connect, message, Disconnect, Ping and Reconnect.
- There are some Client based reserved events like Connect, connect- error, connect-timeout and Reconnect etc.

## Question

1. **What is the benefit of transforming data into packets?**

enable new innovations, services, and business opportunities.

2. **UDP is often refereed to as a connectionless protocol. Why is this?**

because it is analogous to sending a letter where you don’t acknowledge receipt.

3. **Can a socket server application have multiple socket connections?**

Multiple connections on the same server can share the same server-side IP/Port pair as long as they are associated with different client-side IP/Port pairs,

4. **Can a socket connection application be connected to multiple socket servers?**

You cannot use a single socket to connect to multiple servers. You must create a separate socket for each connection.

5. **Can an application be both a socket server and a socket connection?**

You can use the same socket for whatever you want, as long as your protocol handles it.

## Term

**observer Pattern** a subscription model in which objects subscribe to an event and get notified when the event occurs.

**Listener** a procedure in JavaScript that waits for an event to occur.

**Event Handler**that invokes a specific piece of code when a particular action happens on an HTML element.

**Event Driven Programming**Everything starts by following an event. The event could be the DOM is loaded, or an asynchronous request that finishes fetching, or a user clicking an element or scrolling the page, or the user types on the keyboard.

**Event Loop** responsible for executing the code, collecting and processing events, and executing queued sub-tasks

**Event Queue** responsible for sending new functions to the stack for processing.

**Call Stack** a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions

**Emit** on() function that allows one or more functions to be attached to named events emitted by the object.

**Raise** throws a user-defined exception
Trigger The trigger() method triggers the specified event and the default behavior of an event (like form submission) for the selected elements.

**Subscribe** observable of interest

**database** a javascript SQL database. It allows you to create a relational database and query it entirely in the browser.
