# Errata 7145 - RFC 7170

- **RFC Title:** Tunnel Extensible Authentication Protocol (TEAP) Version 1
- **RFC Publication Date:** May 2014

```
Section 3.3.3 says:


   The Crypto-Binding TLV MUST be exchanged and verified

   before the final Result TLV exchange, regardless of whether or not

   there is an inner EAP method authentication.

// state how to fix the above text here

```

## Issue description

The mandate in Section 3.3.3 is not taking its following text into account. This inconsistency creates ambiguity in the specification, impacting implementation.
