# Errata 6178 - RFC 7807

- **RFC Title:** Problem Details for HTTP APIs
- **RFC Publication Date:** March 2016

```
Section 3 says:


   The ability to convey problem-specific extensions allows more than

   one problem to be conveyed.  For example:



   HTTP/1.1 400 Bad Request

   Content-Type: application/problem+json

   Content-Language: en



   {

   "type": "https://example.net/validation-error",

   "title": "Your request parameters didn't validate.",

   "invalid-params": [ {

                         "name": "age",

                         "reason": "must be a positive integer"

                       },

                       {

                         "name": "color",

                         "reason": "must be 'green', 'red' or 'blue'"}

                     ]

   }

// state how to fix the above text here

```

## Issue description

The example in Section 3 uses a member name that is inconsistent with the naming guidelines specified in Section 4. This inconsistency affects the interoperability and correctness of problem details implementations.
