# Errata 5703 - RFC 8422

- **RFC Title:** Elliptic Curve Cryptography (ECC) Cipher Suites for Transport Layer Security (TLS) Versions 1.2 and Earlier
- **RFC Publication Date:** August 2018

```
Section 5.10. says:


All RSA signatures must be generated and verified according to

   Section 7.2 of [RFC8017].

// state how to fix the above text here

```

## Issue description

The original text references the wrong encryption scheme for RSA signature generation and verification. This inconsistency between the referenced section and the expected signature scheme affects the correct implementation of RSA signatures.
