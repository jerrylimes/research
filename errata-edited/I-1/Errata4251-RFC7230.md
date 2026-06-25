# Errata 4251 - RFC 7230

- **RFC Title:** Hypertext Transfer Protocol (HTTP/1.1): Message Syntax and Routing
- **RFC Publication Date:** June 2014

```
Section 2.7.1 says:


     http-URI = "http:" "//" authority path-abempty [ "?" query ]

                [ "#" fragment ]


// state how to fix the above text here



```

## Issue description

The `http-URI` ABNF production in Section 2.7.1 of RFC 7230 includes a component that is not permitted by RFC 3986's requirements for absolute URIs, creating an inconsistency that affects how HTTP clients and servers parse and generate HTTP URIs.
