# Errata 4938 - RFC 7714

- **RFC Title:** AES-GCM Authenticated Encryption in the Secure Real-time Transport Protocol (SRTP)
- **RFC Publication Date:** December 2015

```
Section 11 says:


A Key Derivation Function (KDF) is used to derive all of the required

encryption and authentication keys from a secret value shared by the

endpoints.  The AEAD_AES_128_GCM algorithm MUST use the (128-bit)

AES_CM PRF KDF described in [RFC3711].  AEAD_AES_256_GCM MUST use the

AES_256_CM_PRF KDF described in [RFC6188].

// state how to fix the above text here

```

## Issue description

The original text does not specify how to handle the 96-bit master salt defined in RFC 7714 with the 112-bit master salt assumed by the KDF functions in RFC 3711.
