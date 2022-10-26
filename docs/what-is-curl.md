**curl**, or **cURL**, is a command line tool used to transfer data to and from a server. It can execute HTTP requests with different parameters and methods.
*[cURL]: client URL

curl lets you talk to a server by specifying the location (in the form of a URL) and the data you want to send.

## curl and REST API documentation
REST APIs can use almost any programming language to call an endpoint. Documenting each programming language would be too time-consuming, so curl can be used to demonstrate the call.

If you make a curl request for a website, curl will retrieve and display the website's code.

For example, the following command:

```html
curl https://example.com
```

returns the following response:


```html
<!doctype html>
    <html>

    <head>
        <title>Example Domain</title>

        <meta charset="utf-8" />
        <meta http-equiv="Content-type" content="text/html; charset=utf-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1" />
        <style type="text/css">
            body {
                background-color: #f0f0f2;
                margin: 0;
                padding: 0;
                font-family: -apple-system, system-ui, BlinkMacSystemFont, "Segoe UI", "Open Sans", "Helvetica Neue", Helvetica, Arial, sans-serif;

            }

            div {
                width: 600px;
                margin: 5em auto;
                padding: 2em;
                background-color: #fdfdff;
                border-radius: 0.5em;
                box-shadow: 2px 3px 7px 2px rgba(0, 0, 0, 0.02);
            }

            a:link,
            a:visited {
                color: #38488f;
                text-decoration: none;
            }

            @media (max-width: 700px) {
                div {
                    margin: 0 auto;
                    width: auto;
                }
            }
        </style>
    </head>

    <body>
        <div>
            <h1>Example Domain</h1>
            <p>This domain is for use in illustrative examples in documents. You may use this
                domain in literature without prior coordination or asking for permission.</p>
            <p><a href="https://www.iana.org/domains/example">More information...</a></p>
        </div>
    </body>

    </html>
```

If you were to request the same website on a browser, then the browser would display the code in a way that’s visually readable.

curl, however, shows you what you're actually retrieving (code).

## curl and Windows
- Always use double-quotes instead of single-quotes
- Don’t use backslashes (`\`) to separate lines
- Add `-k` to the curl command to bypass curl’s security certificate (if necessary)

## How to confirm if you have curl installed
Run the following command from the command line:

```html
curl --version
```

The response should look like this:

```html
curl 7.83.1 (Windows) libcurl/7.83.1 Schannel
Release-Date: 2022-05-13
Protocols: dict file ftp ftps http https imap imaps pop3 pop3s smtp smtps telnet tftp
Features: AsynchDNS HSTS IPv6 Kerberos Largefile NTLM SPNEGO SSL SSPI UnixSockets
```

***

##### Sources
- [Documenting APIs: A guide for technical writers and engineers](https://idratherbewriting.com/learnapidoc/) by Tom Johnson
- [curl.se](https://curl.se/)
- ["What is cURL and how does it relate to APIs?"](https://developer.ibm.com/articles/what-is-curl-command/) from IBM Developer
