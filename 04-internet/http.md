# 5. What Actually Happens on the Internet? (continued)

### 45. Why do we need ports?
An IP address identifies a network interface, while a port identifies a communication endpoint associated with a service on that device. Together, an address and port help network software deliver traffic to the right application.

### 46. What is HTTP?
HTTP is an application-layer protocol for exchanging requests and responses, commonly between browsers and web servers. Requests include a method and target, and responses include a status code; headers and optional bodies carry additional information.

### 48. What happens when you click a button on a website?
The browser runs the button's associated behavior, which may update the page, validate input, or send a network request. If it contacts a server, the browser sends an HTTP request and uses the response to update the interface.

### 50. How does the server know where to send the response?
The network connection records the client endpoint, including its address and port, so the response can be sent back over that connection. At the application level, the server's response is also associated with the request that produced it.