# Errata 5868 - RFC 8446

- **RFC Title:** The Transport Layer Security (TLS) Protocol Version 1.3
- **RFC Publication Date:** August 2018

```
Section 4.2.3 says:


   ECDSA algorithms:  Indicates a signature algorithm using ECDSA

      [ECDSA], the corresponding curve as defined in ANSI X9.62 [ECDSA]

      and FIPS 186-4 [DSS], and the corresponding hash algorithm as

      defined in [SHS].  The signature is represented as a DER-encoded

      [X690] ECDSA-Sig-Value structure.

// state how to fix the above text here

```

## Issue description

The original description of ECDSA signature representation is ambiguous as the ECDSA-Sig-Value structure has multiple definitions.
