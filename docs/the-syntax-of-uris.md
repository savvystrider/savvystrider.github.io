> A **URI** is a string that refers to a resource.
>
> The most common URIs are **URLs**, which identify the resource by giving its location on the Web.
>
> A URL is composed of different parts; some are mandatory and others are optional.
*[URI]: Uniform Resource Indicator
*[URL]: Uniform Resource Locator

### Scheme or protocol 

> `http://example.com`

`http://` is the *protocol*.

It indicates which protocol (HTTP or HTTPS) the browser must use.

### Authority
> `http://example.com`

`www.example.com` is the domain name, or *authority*, that governs the namespace.

It indicates which Web server is being requested.

### Port
> `http://www.example.com:80/path`

`:80` is the *port*.

- It indicates the technical "gate" used to access the resources on the web server.
- It is usually omitted if the web server uses the standard ports of the HTTP protocol (80 for HTTP and 443 for HTTPS) to grant access to its resources.

### Path
 > `http://www.example.com:80/path/to/myfile.html?key1=value1`

 `/path/to/myfile.html` is the *path* to the resource on the Web server.

 Previously, a path like this represented a physical file location on a web server. Now, it is mostly an abstraction handled by web servers without any physical reality.

### Query
> `http://www.example.com:80/path/to/myfile.html?key1=value1&key2=value2`

`key1=value1&key2=value2` are extra *parameters* provided to the web server.

- The parameters are a list of key/value pairs separated with the `&` symbol.
    - Parameters define the search criteria used by the server to find a set of matching resources. 
- The `?` before the key/value pairs indicates the start of the *query string*.

### Fragment
> `http://www.example.com:80/path/to/myfile.html?key1=value1&key2=value2#SomewhereInTheDocument`

`#SomewhereInTheDocument` is an anchor to another part of the resource itself.

An anchor is similar to a "bookmark" inside the resource, giving the browser the directions to show the content located at that "bookmarked" spot.

***

##### Sources
- [MDN Web Docs](https://developer.mozilla.org/en-US/)
- [Documenting APIs: A guide for technical writers and engineers](https://idratherbewriting.com/learnapidoc/) by Tom Johnson
- ["Introduction to RESTful Web services"](https://developer.ibm.com/articles/ws-restful/?mhsrc=ibmsearch_a&mhq=uri) - IBM Developer