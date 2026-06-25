# Errata 6435 - RFC 8536

- **RFC Title:** The Time Zone Information Format (TZif)
- **RFC Publication Date:** February 2019

```
Section 5.2 says:


   >> Response <<



   HTTP/1.1 200 OK

   Date: Fri, 01 Jun 2018 14:52:23 GMT

   Content-Type: application/json; charset="utf-8"

   Content-Length: xxxx

// state how to fix the above text here

```

## Issue description

The original response is missing a parameter in one of the headers for application/json, which is incorrect according to Section 11 of RFC 8259.
