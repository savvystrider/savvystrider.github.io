### API
A set of definitions and protocols that allow technology products and services to communicate via the internet.

### Application state
Information about the client’s path through an API.

### Client
A computer used by a user to connect to a network and make requests to servers.

### Endpoint
The endpoint of an API is a digital location where an API receives requests about a specific resource on its server. In APIs, an endpoint is typically a uniform resource locator (URL) that provides the location of a resource on the server.

### HATEOAS
One of the constraints of REST laid out by Roy Fielding. A server offers a client a "menu" of hypermedia options that a client can choose from.

### HTTP
The underlying network protocol that enables transfer of hypermedia documents on the Web, typically between a browser and a server so that humans can read them.

### HTTP methods / verbs
Options given to a client for requesting or manipulating resources.
Options include: `GET`, `HEAD`, `POST`, `PUT`, `DELETE`, `CONNECT`, `OPTIONS`, `TRACE`, and `PATCH`.

### Idempotent / idempotency
An HTTP method is idempotent if an identical request can be made more than once with the same effect *without* changing the state of the server. A `GET` method is considered idempotent. A `POST` (create) method is not considered idempotent.

### Representation
A piece of data that describes the state of a resource.

### Resource
In general, a resource is whatever might be identified by a URI (documents, files, images, data, etc.)

### REST
Representational State Transfer

### REST API
A web service that makes requests for resources through URL paths.

### Server
A computer that serves many kinds of information to a user or client machine.

### State
Remembered information in a computer system.

### Stateless
In the client-server model, a stateless protocol means that the server does not keep any data (state) between two requests.
This is in contrast to a *stateful* protocol, which does keep data (state) between separate requests.

### URL
A type of URI that identifies a resource *and* provides a means of locating the resource.

### URI
Provides a simple and extensible means for *identifying* a resource. The identifier consists of a string of characters matching syntax rules. A URL is a type of URI.

*[API]: Application programming interface
*[HATEOAS]: Hypermedia as the engine of application state
*[REST]: Representational State Transfer
*[HTTP]: Hypertext Transfer Protocol
*[URI]: Uniform Resource Indicator
*[URL]: Uniform Resource Locator

***

##### Sources
- Fielding, R., Gettys, J., Mogul, J., Frystyk, H., Masinter, L., Leach, P., and T. Berners-Lee, "Hypertext Transfer Protocol -- HTTP/1.1", RFC 2616, DOI 10.17487/RFC2616, June 1999, <https://www.rfc-editor.org/info/rfc2616>.
- [MDN Web Docs](https://developer.mozilla.org/en-US/)
- Richardson, L., & Ruby, S. (2013). *RESTful web apis*.