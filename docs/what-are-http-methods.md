# What are HTTP methods?

**HTTP** is a *request-response protocol* between a client and a server.
*[HTTP]: Hyptertext Transfer Protocol

**HTTP methods** indicate what action should be performed for requesting a specific resource.

These methods are also called *HTTP verbs*. The resource is the *noun*.

**CRUD** refers to the ways that stored data can be operated.

It also refers to the four basic functions of persistent storage and maps to the four major HTTP methods (see below).
*[CRUD]: Create, Read, Update, Delete

HTTP request methods can be:

- **Safe**: methods are safe if they do not alter the state of the server (read-only operation).

- **Idempotent**: methods are idempotent if an identical request can be made (once or more) without changing the original result (i.e., no side effects).

- **Cacheable**: methods can be cached (stored for retrieval), saving a new request to the server.

## HTTP Methods

### `GET`

**Read** / **request** data from a resource.

Safe / idempotent / cacheable

### `POST`

**Create** a resource.

Not safe / Not idempotent / Not cacheable

### `PUT`

**Update** a resource.

Not safe / Idempotent / Not cacheable

### `DELETE`

**Remove** a resource.

Not safe / Idempotent / Not cacheable

### `HEAD`

**Read** / **request** data (same as `GET`) from a resource but without a response body.

Safe / idempotent / cacheable

### `PATCH`

Apply partial modifications to a resource.

Not safe / Not idempotent / Not cacheable

### `OPTIONS`

Describe the communication options for a resource.

Safe / Idempotent / Not cacheable

### `CONNECT`

Establish a tunnel to the server identified by a resource.

Not safe / Not idempotent / Not cacheable

### `TRACE`

Perform a message loop-back test along the path to a resource.

Safe / Idempotent / Not cacheable

***

##### Sources
- [Documenting APIs: A guide for technical writers and engineers](https://idratherbewriting.com/learnapidoc/) by Tom Johnson
- [The IETF HTTP Working Group](https://httpwg.org/)
- [MDN Web Docs](https://developer.mozilla.org/en-US/)