# 5. What Actually Happens on the Internet? (continued)

### 42. How does your computer find Google’s server?
DNS provides an address for the domain; routers then forward packets toward that destination using network routing. The destination may be a nearby edge server or a service behind a load balancer, not one permanently fixed machine.

### 44. What is an IP address?
An Internet Protocol address identifies a network interface on an IP network so packets can be routed toward it. IPv4 and IPv6 use different address formats; addresses can be public or private and may change over time.

### 49. How does your request travel thousands of kilometres?
The request is split into packets carried over interconnected networks. Routers forward packets hop by hop using routing tables; the path can vary, and lower-level technologies carry the packets across local links, cables, and wireless networks.