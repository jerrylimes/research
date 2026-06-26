# Errata 7736 - RFC 9085

- **RFC Title:** Border Gateway Protocol - Link State (BGP-LS) Extensions for Segment Routing
- **RFC Publication Date:** August 2021

```
Section 2.3.5 says:


   A Prefix NLRI, that has been advertised with a Range TLV, is

   considered a normal routing prefix (i.e., prefix reachability) only

   when there is also an IGP metric TLV (TLV 1095) associated it.

   Otherwise, it is considered only as the first prefix in the range for

   prefix-to-SID mapping advertisement.

// state how to fix the above text here

```

## Issue description

The current text is referring to the wrong BGP-LS TLV and contains a grammatical mistake. This inconsistency could affect implementations that rely on the correct TLV to identify normal routing prefixes.
