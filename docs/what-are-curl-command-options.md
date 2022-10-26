curl has over 200 command options. The most basic command in curl is: 

```html
curl http://example.com
```

where the command (`curl`) is followed by the URL.

This is a summary of the commands most relevant to API documentation:

### **`i, --include`**
- Include the HTTP response headers in the output.
- The `verbose` option is also available.

`curl -i https://example.com`

***

### **`-I, --head`**
Only include the HTTP response headers in the output.

`curl -I https://example.com`

***

### **`-H, --header <header/@file>`**
Include extra or custom headers.

`curl -H "X-First-Name: Joe" https://example.com`

`curl -H "User-Agent: yes-please/2000" https://example.com`

`curl -H "Host:" https://example.com`

***

### **`-v, --verbose`**
Useful for debugging and getting additional information about what has been sent/received.

`curl --verbose https://example.com`

***

### **`-d, --data <data>`**
Sends the specified data in a `POST` request to the HTTP server, in the same way that a browser does when a user has filled in an HTML form and presses the submit button.

`curl -d "name=curl" https://example.com`

`curl -d "name=curl" -d "tool=cmdline" https://example.com`

`curl -d @filename https://example.com`

***

### **`-G, --get`**
Retrieve a resource from a server.

`curl --get https://example.com`

***

### **`-k, --insecure`**
- By default, every secure connection curl makes is verified to be secure before the transfer takes place. This option makes curl skip the verification step and proceed without checking.

`curl --insecure https://example.com`

***

### **`-L, --location`**
Submits a new request if the URL is a redirect.

`curl -L https://example.com`

***

### **`-X, --request <method>`**
Specifies a custom request method to use when communicating with the HTTP server. The specified request method will be used instead of the method otherwise used (which defaults to `GET`).

`curl -X "DELETE" https://example.com`

***

##### Sources
- [Documenting APIs: A guide for technical writers and engineers](https://idratherbewriting.com/learnapidoc/) by Tom Johnson
- [curl.se](https://curl.se/)
- ["What is cURL and how does it relate to APIs?"](https://developer.ibm.com/articles/what-is-curl-command/) from IBM Developer