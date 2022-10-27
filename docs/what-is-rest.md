**REST** is an *architectural-style* that refers to more than just APIs. REST describes how a client and a server can interact using HTTP as their form of communication.

Think about about what happens when you open a web browser and type in a URL (`http://`...). What's on the other end of that URL?

A **resource**, that's what. That resource is a representation of something. It's not the thing itself, just a representation of that thing.

Trying to download a photo of a dog on a skateboard doesn't actually give you a dog on a skateboard. Just a representation of a dog on a skateboard.

Each URL identifies a resource. Or, that's how it's supposed to work. Real life and the internet can both be complicated.

Anyway, a client makes an HTTP request to a URL for a resource and receives a representation of that resource in the form of a response.

Once the client receives the response, the request is over, and it's almost as if it never happened.

REST is defined by four uniform interface constraints:

1. Identifying named resources (data) for requests. These resources are made available through **URIs**. A URL is a type of URI.

2. The ability to modify or delete the representations of these resources.

3. Self-descriptive messages. Clients and servers can exchange messages with enough information to process each request and response. 

4. HATEOAS, a fun acronym that describes how hypermedia is served up to a client like a menu, offering the client all the information they need to make requests.

*[REST]: Representational State Transfer
*[HATEOAS]: Hypermedia as the Engine of Application State
*[URI]: Uniform Resource Indicator
*[HTTP]: Hypertext Transfer Protocol
*[hypermedia]: Data sent from the server to the client, which explains what the client can do next.  


***

##### Sources
- Fielding, Roy Thomas. *Architectural Styles and the Design of Network-based Software Architectures*. Doctoral dissertation, University of California, Irvine, 2000.
- Fielding, R., Gettys, J., Mogul, J., Frystyk, H., Masinter, L., Leach, P., and T. Berners-Lee, "Hypertext Transfer Protocol -- HTTP/1.1", RFC 2616, DOI 10.17487/RFC2616, June 1999, <https://www.rfc-editor.org/info/rfc2616>.
- Richardson, L., & Ruby, S. (2013). *RESTful web apis*. 