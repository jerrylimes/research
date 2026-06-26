# Errata 7419 - RFC 97

- **RFC Title:** HTTP Semantics
- **RFC Publication Date:** June 2022

```
Section 8.3.2 says:


   In the fields defined by this document, charset names appear either

   in parameters (Content-Type), or, for Accept-Encoding, in the form of

   a plain token.

// state how to fix the above text here

```

## Issue description

The text in Section 8.3.2 refers to the incorrect list that contains charset names in the form of a plain token. This directly affects the correct interpretation of how charset names are used, leading to potential implementation errors.
