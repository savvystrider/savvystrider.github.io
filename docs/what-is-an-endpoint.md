REST APIs focus on *resources* and how to *access* those resources.

Resources are accessed through endpoints.

An **endpoint** is the address (URL), or *location*, of the resource.

These resources can be accessed through **HTTP methods**:
- `GET` - read
- `POST` - create
- `PUT` - update
- `DELETE` - delete

The endpoint usually includes **query parameters** that specify more information about the representation of the requested resource.

For example, you can specify (in a query parameter) that you want to limit the display to 5 instances of the resource (see example below).

## Sample endpoint:

`http://apiserver.com/homes?limit=5&format=json`

> **Base path**: `http://apiserver.com`
>
> **Endpoint**: `/homes`
>
> **Query string parameters**: `?limit=5&format=json`

***

##### Sources
- [Documenting APIs: A guide for technical writers and engineers](https://idratherbewriting.com/learnapidoc/) by Tom Johnson
- ["What is cURL and how does it relate to APIs?"](https://developer.ibm.com/articles/what-is-curl-command/) from IBM Developer