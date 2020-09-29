## Socket IO

### What is WebSockets ?
**WebSocket** is a computer communication protocol which provides full-duplex communication channels over a single TCP connection.
- It is different from HTTP but compatible with HTTP.
- Located at layer 7 in the OSI model and depends on TCP at layer 4.
- Works over port 80 and 443 ( in case of TLS encrypted) and supports HTTP proxies and intermediaries.
- To achieve compatibility, the WebSocket handshake uses Upgrade header to update the protocol to the WebSocket protocol.

<img src="https://files.ably.io/ghost/prod/2020/08/Websockets.gif" />

### What Socket.IO is ?
**Socket.IO** is a library that enables real-time, bidirectional and event-based communication between the browser and the server. `It consists of`:
- a Node.js server:
- a Javascript client library for the browser (which can be also run from Node.js):

### Socket.IO namespaces
Socket.IO allows you to **“namespace”** your sockets, which essentially means assigning different endpoints or paths. This is a useful feature to minimize the number of resources (TCP connections) and at the same time separate concerns within your application by introducing separation between communication channels. Multiple namespaces actually share the same WebSockets connection thus saving us socket ports on the server.

`Default Namespaces`
The root namespace '/' is the default namespace,
```Javascript
var socket = io();
```

### Socket.IO Applications
A real-time application (RTA) is an application that functions within a period that the user senses as immediate or current.
<br/>
- **Instant messengers** − Chat apps like Whatsapp, Facebook Messenger, etc. You need not refresh your app/website to receive new messages.
- **Push Notifications** − When someone tags you in a picture on Facebook, you receive a notification instantly.
- **Collaboration Applications** − Apps like google docs, which allow multiple people to update same documents simultaneously and apply changes to all people's instances.
- **Online Gaming** − Games like Counter Strike, Call of Duty, etc., are also some examples of real-time applications.
