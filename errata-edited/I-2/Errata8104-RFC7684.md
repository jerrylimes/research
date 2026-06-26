# Errata 8104 - RFC 7684

- **RFC Title:** OSPFv2 Prefix/Link Attribute Advertisement
- **RFC Publication Date:** November 2015

```
Section 2.1 says:


   Route Type

      The type of the OSPFv2 route.  If the route type is 0

      (Unspecified), the information inside the OSPFv2 External Prefix

      TLV applies to the prefix regardless of prefix's route type.  This

      is useful when prefix-specific attributes are advertised by an

      external entity that is not aware of the route type associated

      with the prefix.  Supported types are:

// state how to fix the above text here

```

## Issue description

The original text refers to the wrong TLV that contains relevant information. This inconsistency creates a mismatch between the description and the actual TLV used, affecting the correct interpretation and implementation of the specification.
