# Errata 5669 - RFC 8152

- **RFC Title:** CBOR Object Signing and Encryption (COSE)
- **RFC Publication Date:** July 2017

```
Section 16.7 says:


Value:  This is the value used to identify the curve.  These values

   MUST be unique.  The value can be a positive integer, a negative

   integer, or a string.



Description:  This field contains a brief description of the curve.



References:  This contains a pointer to the public specification for

   the curve if one exists.

// state how to fix the above text here

```

## Issue description

The original description of the registry entries does not correctly identify what the registry is for, and, as a result, incorrectly states the type of the value used to identify it. This inconsistency affects the interpretation and use of the key type registry.
