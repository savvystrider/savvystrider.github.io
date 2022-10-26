**HTTP messages** are how data is exchanged between a server and a client.

- Two types of messages:

- **requests**, sent by the client to trigger an action on the server.

- **responses**, the answer from the server.

- Clients and servers communicate by exchanging individual messages (as opposed to a stream of data). 

- Messages are human-readable.

## Structure of requests and responses

![HTTP message structure](https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages/httpmsgstructure2.png)

HTTP requests and responses share a similar structure and include:

1. a **start-line** that describes the request being made, or its success status. Always a single line.

2. optional HTTP **headers** for specifying the request or describing the body included in the message.

    Header fields are key-value pairs separated by colons.

3. a **blank line** indicating all meta-information for the request has been sent.

4. an optional **body** that contains data associated with the request or the document associated with the response.

***

## HTTP Request

![HTTP request](https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview/http_request.png)

**HTTP Method**

Defines the operation the client wants to perform. Options include:
- `GET`
- `POST`
- `PUT`
- `DELETE`

**Path**

The path of the requested resource.

**Version**

Version of HTTP protocol

**Headers**

Optional headers to convey additional information for the servers

**Body**

A `POST` method would contain the resource being sent to the server.

***

## HTTP Response

![HTTP response](https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview/http_response.png)

**Version**

Version of HTTP protocol

**Status code**

Indicates whether a specific HTTP request has been successfully completed.

**Status message**

A non-authoritative short description of the status code.

**Headers**

HTTP headers, like those for requests.

Header fields are key-value pairs separated by colons.

**Body**

Optional. Contains the fetched resource.

***

##### Sources
- [MDN Web Docs](https://developer.mozilla.org/en-US/)