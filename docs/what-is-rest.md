**REST** is an *architectural-style* that refers to more than just APIs. REST describes how a client and a server can interact using HTTP as the form of communication.

Think about about what happens when you open a web browser and type in a URL (http://...). What's on the other end of that URL?

A resource, that's what. That resource is a representation of something. It's not the thing itself, just a representation of that thing.

Each URL identifies a resource. A client makes an HTTP request to a URL for a resource and receives a representation of that resource in the form of a response.

Once the client receives the response, the request is over. 

REST is defined by four uniform interface constraints:

1. Identifying named resources (data) for requests. These resources are available through **URIs**.

2. The ability to modify or delete the representations of these resources.

3. Self-descriptive messages. Clients and servers exchange messages with enough information to process each request and response. 

4. HATEOAS - 

*[REST]: Representational State Transfer
*[HATEOAS]: Hypermedia as the Engine of Application State
*[URI]: Uniform Resource Indicator
*[HTTP]: Hypertext Transfer Protocol  


***

##### Sources
- Fielding, Roy Thomas. *Architectural Styles and the Design of Network-based Software Architectures*. Doctoral dissertation, University of California, Irvine, 2000.
- Fielding, R., Gettys, J., Mogul, J., Frystyk, H., Masinter, L., Leach, P., and T. Berners-Lee, "Hypertext Transfer Protocol -- HTTP/1.1", RFC 2616, DOI 10.17487/RFC2616, June 1999, <https://www.rfc-editor.org/info/rfc2616>.