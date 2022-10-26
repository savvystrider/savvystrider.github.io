## Status Line
The **status line** is the first/starting line of an HTTP response. It contains the following information:
- the protocol version.
- a status code, which indicates success or failure of the request.
- a status text, which provides a text description.

A typical status line looks like this: `HTTP/1.1 404 Not Found`

## Headers

![HTTP response headers](https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages/http_response_headers3.png)

**HTTP headers** let the client and the server pass additional information with an HTTP request or response.

Headers are in key-value pairs separated by a colon. Example:

`key`: `value`

A **representation header** is a type of HTTP header that describes the particular representation of the resource sent in an HTTP message body. Example:

`Content-Length`: `100`

## Body

The **body** is the final part of an HTTP response. Not all responses need one.

***

##### Sources
- [MDN Web Docs](https://developer.mozilla.org/en-US/)