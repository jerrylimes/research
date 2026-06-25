# Errata 5622 - RFC 8306

- **RFC Title:** Extensions to the Path Computation Element Communication Protocol (PCEP) for Point-to-Multipoint Traffic Engineering Label Switched Paths
- **RFC Publication Date:** November 2017

```
Section 3.13 says:


   The total PCEP message length, including the common header, is

   16 bytes.

// state how to fix the above text here

```

## Issue description

The original text incorrectly states the length of the PCEP message field.  This inconsistency would lead to implementations incorrectly limiting the maximum PCEP message size. For reference, check Section 6.1 of RFC5440.
