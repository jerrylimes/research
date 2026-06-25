# Errata 7014 - RFC 9114

- **RFC Title:** HTTP/3
- **RFC Publication Date:** June 2022

```
Section 4.3.1 says:


   ":path":  Contains the path and query parts of the target URI (the

      "path-absolute" production and optionally a ? character (ASCII

      0x3f) followed by the "query" production; see Sections 3.3 and 3.4

      of [URI].

// state how to fix the above text here

```

## Issue description

The description of a header field in Section 4.3.1 conflicts with the usage in other RFCs (RFCs 9110, 9112, 9113) and the intended behavior. This inconsistency affects interoperability, as implementations might interpret the path differently based on which RFC they adhere to more strictly.
