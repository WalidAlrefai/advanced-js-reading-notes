# Message Queues

1. **What does it mean that web sockets are bidirectional? Why is this useful?**

Means that BIDIRECTIONAL websocket, WebSockets allow full-duplex bidirectional communication. This enables the server to send real-time updates asynchronously, without requiring the client to submit a request each time.

2. **Does socket.io use HTTP? Why?**

Yes, It does, and will use HTTP long-polling as fallback.

3. **What happens when a client emits an event?**

It fires events in the server and it listen to events

4. **What happens when a server emits an event?**

This events fires for all the clients that connected to this server. With

5. **What happens if a client “misses” an event?How can we mitigate this?**

When mistakes happen it’s important to be honest and identify where errors have occurred.


# Term

- **Socket:**is used in a client-server application framework. A server is a process that performs some functions on request from a client.
- **Web Socket:**is a computer communications protocol, providing full-duplex communication channels over a single TCP connection.
- **Socket.io:** is a JavaScript library for realtime web applications. It enables realtime, bi-directional communication between web clients and servers. It has two parts: a client-side library that runs in the browser, and a server-side library for Node.js.
- **Client:** which means the source code is processed by the client's web browser rather than on the web server. This means JavaScript functions can run after a webpage has loaded without communicating with the server.
- **Server:** is a piece of computer hardware or software (computer program) that provides functionality for other programs or devices, called "clients". This architecture is called the client–server model. Servers can provide various functionalities, often called "services"
- **OSI Model:** The Open Systems Interconnection model (OSI model) is a conceptual model that characterises and standardises the communication functions of a telecommunication or computing system without regard to its underlying internal structure and technology. Its goal is the interoperability of diverse communication systems with standard communication protocols.
- **TCP Model:** is the set of communications protocols used in the Internet and similar computer networks. The current foundational protocols in the suite are the Transmission Control Protocol (TCP) and the Internet Protocol (IP).
- **TCP:** The Transmission Control Protocol (TCP) is one of the main protocols of the Internet protocol suite. It originated in the initial network implementation in which it complemented the Internet Protocol (IP). Therefore, the entire suite is commonly referred to as TCP/IP.
- **UDP:** User Datagram Protocol (UDP) is a Transport Layer protocol. UDP is a part of the Internet Protocol suite, referred to as UDP/IP suite. Unlike TCP, it is an unreliable and connectionless protocol. So, there is no need to establish a connection prior to data transfer.
- **Packets:** is a formatted unit of data carried by a packet-switched network. A packet consists of control information and user data; the latter is also known as the payload.
