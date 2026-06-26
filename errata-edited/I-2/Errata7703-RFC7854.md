# Errata 7703 - RFC 7854

- **RFC Title:** BGP Monitoring Protocol (BMP)
- **RFC Publication Date:** June 2016

```
Section 4.2 says:


      *  The L flag, if set to 1, indicates that the message reflects

         the post-policy Adj-RIB-In (i.e., its path attributes reflect

         the application of inbound policy).  It is set to 0 if the

         message reflects the pre-policy Adj-RIB-In.  Locally sourced

         routes also carry an L flag of 1.  See Section 5 for further

         detail.  This flag has no significance when used with route

         mirroring messages (Section 4.7).

// state how to fix the above text here

```

## Issue description

The original description does not correctly describe when and for what the L flag has significance. This inconsistency between the original description and the actual usage of the L flag could lead to misinterpretations and incorrect implementations.
