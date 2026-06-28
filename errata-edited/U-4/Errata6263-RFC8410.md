# Errata 6263 - RFC 8410

- **RFC Title:** Algorithm Identifiers for Ed25519, Ed448, X25519, and X448 for Use in the Internet X.509 Public Key Infrastructure
- **RFC Publication Date:** August 2018

```
Section 7 says:


NOTE: There exist some private key import functions that have not picked up the new ASN.1 structure OneAsymmetricKey that is defined in [RFC7748].

// state how to fix the above text here

```

## Issue description

The original text incorrectly cites RFC 7748 as the source for the OneAsymmetricKey ASN.1 structure. This inconsistency would affect those trying to locate the correct ASN.1 definition.
