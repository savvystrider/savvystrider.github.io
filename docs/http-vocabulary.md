### Client
A computer used by a user to connect to a network and make requests to servers.

### CRUD
The four basic operations of persistent storage, in computer programming.

These operations map to the four main HTTP methods: create/`POST`, read/`GET`, update/`PUT`, and DELETE/`DELETE`.

### HTTP
The underlying network protocol that enables transfer of hypermedia documents on the Web, typically between a browser and a server so that humans can read them.

### HTTP header
Allows clients and servers to pass additional information to each other with HTTP requests and HTTP responses.

### HTTP messages
How data is exchanged between a client and a server.

There are two types of HTTP messages: HTTP *requests*, sent by a client to a server, and HTTP *responses*, sent from the server to the client.

### HTTP methods / verbs
Options given to a client for requesting or manipulating resources.

Options include: `GET`, `HEAD`, `POST`, `PUT`, `DELETE`, `CONNECT`, `OPTIONS`, `TRACE`, and `PATCH`.

### HTTP request
HTTP messages sent by the client to initiate an action on the server.

### HTTP response
HTTP messages sent from a server to the client, which can include a representation of a resource, a success message, or an error message.

### HTTP response status codes
HTTP messages sent from a server indicating whether a client's HTTP request is successful.

### Idempotent / idempotency
An HTTP method is idempotent if an identical request can be made more than once with the same effect *without* changing the state of the server. A `GET` method is considered idempotent. A `POST` (create) method is not considered idempotent.

### Protocol
A system of rules that define how data is exchanged within or between computers.

### Server
A computer that serves many kinds of information to a user or client machine.

### Stateless
In the client-server model, a stateless protocol means that the server does not keep any data (state) between two requests.

This is in contrast to a *stateful* protocol, which does keep data (state) between separate requests.

HTTP is a stateless protocol.

*[API]: Application programming interface
*[HATEOAS]: Hypermedia as the engine of application state
*[REST]: Representational State Transfer
*[HTTP]: Hypertext Transfer Protocol
*[URI]: Uniform Resource Indicator
*[URL]: Uniform Resource Locator
*[CRUD]: Create, Read, Update, Delete

***

##### Sources
- Fielding, R., Gettys, J., Mogul, J., Frystyk, H., Masinter, L., Leach, P., and T. Berners-Lee, "Hypertext Transfer Protocol -- HTTP/1.1", RFC 2616, DOI 10.17487/RFC2616, June 1999, <https://www.rfc-editor.org/info/rfc2616>.
- [MDN Web Docs](https://developer.mozilla.org/en-US/)
- Richardson, L., & Ruby, S. (2013). *RESTful web apis*.