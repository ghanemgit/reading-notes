# WRRC and Java

## The HTTP Request Lifecycle
### We can summarize the HTTP lifecycle by these steps
#### 1- Local Processing
- In this step the processing depend on the application that does it, Imagine that we use A browser first the browser extracts the "scheme"/protocol (we have established that this will be HTTP), the browser will then look through its own cache of recently requested URLs, the operating system’s cache of recent queries, your router’s cache, and your DNS cache.
#### 2- Resolve an IP
- If the cache lookup fails the browser create a DNS request using [UDP](https://en.wikipedia.org/wiki/User_Datagram_Protocol), The DNS request contains the preconfigured IP for your DNS server and your return IP in its header.Your request will now have to travel many network devices to reach its target DNS server, after that the server looks for the address associated with the requested hostname. If it finds one, it sends a response. If, on the other hand, the DNS server you have targeted cannot locate the given hostname, after request successfully done If the response makes it back the requesting client now has a target IP.
#### 3-Establish a TCP Connection
- To establish a connection, TCP uses a three-way handshake. Before a client attempts to connect with a server, the server must first bind to and listen at a port to open it up for connections: this is called a passive open. Once the passive open is established, a client may initiate an active open.
#### 4- Send an HTTP Request
- The request is made up of a "request line", request header, and a body. The "request line" is simply a line that indicates the HTTP method, the resource being requested, and the protocol version.Once the HTTP request is sent, it follows a similar routing procedure as the one discussed earlier next, the server receives the request, processes it, and finds the resource being requested, it generates an HTTP response. when the response is generated, the server responds to the request.
#### 5- Tearing Down and Cleaning Up
- Once the response has been fully delivered, the client sends a FIN packet at the TCP level, to which the server responds with an ACK, and then generally sends a FIN of its own, At this point, your browser begins processing what it has received. If it is an image, data, or other media file that is being consumed by some application inside the browser.


## High-level HTTP
#### In this quick Reading, we present a way of performing HTTP requests in Java by using the built-in Java class `HttpUrlConnection`.
### HttpUrlConnection
#### The HttpUrlConnection class allows us to perform basic HTTP requests without the use of any additional libraries. All the classes that we need are part of the java.net package.The disadvantages of using this method are that the code can be more heavy than other HTTP libraries. thats done by create an HttpUrlConnection instance using the openConnection() method of the URL class.
#### The HttpUrlConnection class is used for all types of requests by setting the requestMethod attribute to one of the values: GET, POST, HEAD, OPTIONS, PUT, DELETE, TRACE.

