# Errata 5483 - RFC 8446

- **RFC Title:** The Transport Layer Security (TLS) Protocol Version 1.3
- **RFC Publication Date:** August 2018

```
Section 4.2.8.2 says:


For X25519 and X448, the contents of the public value are the byte

string inputs and outputs of the corresponding functions defined in

[RFC7748]: 32 bytes for X25519 and 56 bytes for X448.

// state how to fix the above text here

```

## Issue description

The original text's specification on the content of the public value is inconsistent with Section 7.4.2 and RFC 7748.
