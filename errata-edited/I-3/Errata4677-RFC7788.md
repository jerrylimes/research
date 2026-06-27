# Errata 4677 - RFC 7788

- **RFC Title:** Home Networking Control Protocol
- **RFC Publication Date:** April 2016

```
Section 8 says:


   A network-wide

   zone is appended to all single labels or unqualified zones in order

   to qualify them. ".home" is the default; however, an administrator

   MAY configure the announcement of a Domain-Name TLV (Section 10.6)

   for the network to use a different one.

// state how to fix the above text here

```

## Issue description

The original text uses a label that has not been officially recognized as the default network-wide zone. This inconsistency could lead to implementations using that label as the default without proper consideration of the process for defining such values.
