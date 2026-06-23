# Errata 7565 - RFC 8555

- **RFC Title:** Automatic Certificate Management Environment (ACME)
- **RFC Publication Date:** March 2019
- Link to original errata report: [rfc-editor.org/errata/eid7565](https://www.rfc-editor.org/errata/eid7565)

```
Section 8.1 says:


 The "Thumbprint" step indicates the computation specified in

   [RFC7638], using the SHA-256 digest [FIPS180-4].  As noted in

   [RFC7518] any prepended zero octets in the fields of a JWK object

   MUST be stripped before doing the computation.

// state how to fix the above text here

```

## Issue description

The description in Section 8.1 is not taking the nature of ECDSA keys into consideration. This inconsistency directly impacts the correct implementation of the thumbprint calculation for ECDSA keys.
