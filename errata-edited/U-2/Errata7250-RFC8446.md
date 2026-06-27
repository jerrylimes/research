# Errata 7250 - RFC 8446

- **RFC Title:** The Transport Layer Security (TLS) Protocol Version 1.3
- **RFC Publication Date:** August 2018

```
Section 4.6.1 says:


   The client MAY use this PSK for future handshakes by including the

   ticket value in the "pre_shared_key" extension in its ClientHello

   (Section 4.2.11).

// state how to fix the above text here

```

## Issue description

The original specification is unclear about how clients that do not support session tickets should handle the presence of the "pre_shared_key" extension. This omission in the original specification leads to ambiguity in implementation.
