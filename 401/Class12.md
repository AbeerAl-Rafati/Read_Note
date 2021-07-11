##  Review  

**What is the benefit of transforming data into packets?**  

to meet the demands of pervasive data-centric applications and services.

**UDP is often refereed to as a connectionless protocol. Why is this?**   
because it is analogous to sending a letter where you don't acknowledge receipt.  


**Can a socket server application have multiple socket connections?**   
quantity can be easily extended by adding additional network interfaces to a server.   

**Can a socket connection application be connected to multiple socket servers?**  
yes as long as each of the sockets on the port is connected to a different remote location   

**Can an application be both a socket server and a socket connection?**  
yes


##  Vocabulary   

| voc                               | related to |
|-------------------------------------|--------------|
|Observer Pattern |The observer pattern is a software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods.|
|Listener|function that is invoked when a particular event occurs, typically with an event object containing information about the event.|
|Event Handler| is an action or occurrence recognized by software, often originating asynchronously from the external environment,|
|Event Driven Programming|is a programming paradigm in which the flow of the program is determined by events such as user actions, sensor outputs, or message passing from other programs or threads.|
|Event Loop|the event loop is a programming construct or design pattern that waits for and dispatches events or messages in a program.|
|Event Queue|repository where events from an application are held prior to being processed by a receiving program or system.|
|Call Stack|mechanism for an interpreter to keep track of its place in a script that calls multiple functions |
|Subscribe|allows you to subscribe to a range of events, and define callback|
|database|optional object of data passed to an event method|
|





## Preview  


*Which 3 things had you heard about previously and now have better clarity on?*  
- events
- Listener


*Which 3 things are you hoping to learn more about in the upcoming lecture/demo?*  
-   events


*What are you most excited about trying to implement or see how it works?*  
- events

&nbsp;

## Preparation Materials

> Web Sockets     

- WebSocket is a computer communications protocol, providing full-duplex communication channels over a single TCP connection.   

- The WebSocket protocol enables interaction between a web browser (or other client application) and a web server with lower overhead than half-duplex alternatives such as HTTP polling, facilitating real-time data transfer from and to the server.   


- WebSocket provides full-duplex communication.[2][3] Additionally, WebSocket enables streams of messages on top of TCP. TCP alone deals with streams of bytes with no inherent concept of a message.    

-  WebSocket protocol specification defines ws (WebSocket) and wss (WebSocket Secure) as two new uniform resource identifier (URI) schemes. that are used for unencrypted and encrypted connections, respectively.

&nbsp;

&nbsp;



> Socket.io vs Web Sockets  

- ***WebSocket*** is the communication Protocol that provides bidirectional communication between the Client and the Server over a TCP connection; WebSocket remains open all the time, so they allow real-time data transfer.   

***features***    
1. WebSocket helps in real-time communication between the Client and the webserver.
2. This protocol helps in transforming to cross-platform in a real-time world between the server and the client.
3. This also enables the business worldwide for a real-time web application to enhance and increase the feasibility.
4. The major advantage it stands over an HTTP connection that it provides full-duplex communication.


***Socket.IO*** is a library that enables real-time and full-duplex communication between the Client and the Web servers. It uses the WebSocket protocol to provide the interface. Generally, it is divided into two parts; both WebSocket vs Socket.io are event-driven libraries.   

***features***    

1. It helps in broadcasting to multiple sockets at a time and handles the connection transparently.
It works on all platform, server or device, ensuring equality, reliability, and speed.
2. It automatically upgrades the requirement to WebSocket if needed.
3. It is a custom real-time transport protocol implementation on top of other protocols.
4. It requires both libraries to be used Client side as well as a server-side library.
5. IO works on work-based events. there are some reserved events that can be accessed using the Socket on the server side like Connect, message, Disconnect, Ping and Reconnect.
6. There are some Client based reserved events like Connect, connect- error, connect-timeout and Reconnect etc.
