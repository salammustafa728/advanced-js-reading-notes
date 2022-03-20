# Message Queues


* **What does it mean that web sockets are bidirectional? Why is this useful?**

Means that BIDIRECTIONAL websocket,  WebSockets allow full-duplex bidirectional communication. This enables the server to send real-time updates asynchronously, without requiring the client to submit a request each time.

* **Does socket.io use HTTP? Why?**

**Yes, It does, and will use HTTP long-polling as fallback.**

* **What happens when a client emits an event?**

It fires events in the server and it listen to events

* **What happens when a server emits an event?**

This events fires for all the clients that connected to this server

* **What happens if a client “misses” an event?How can we mitigate this?**

When mistakes happen it’s important to be honest and identify where errors have occurred


**Socket.io Chat Example**

its a basic chat example requires almost no basic prior knowledge of Node.JS or Socket.IO


[Home](../README.md)