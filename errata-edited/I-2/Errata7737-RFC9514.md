# Errata 7737 - RFC 9514

- **RFC Title:** Border Gateway Protocol - Link State (BGP-LS) Extensions for Segment Routing over IPv6 (SRv6)
- **RFC Publication Date:** December 2023

```
Section 5.1 says:


   The IPv6 Prefix matching the locator may also be advertised as prefix

   reachability by the underlying routing protocol.  In this case, the

   Prefix NLRI would also be associated with the Prefix Metric TLV

   [RFC7752] that carries the routing metric for this prefix.  A Prefix

   NLRI that has been advertised with a SRv6 Locator TLV is also

   considered a normal routing prefix (i.e., prefix reachability) only

   when there is also an IGP Metric TLV (TLV 1095) associated it.

   Otherwise, it is only considered an SRv6 Locator advertisement.

// state how to fix the above text here

```

## Issue description

The original text refers to the incorrect TLV for Prefix NLRIs and contains a grammatical mistake. This inconsistency could affect implementations that rely on the correct TLV to identify normal routing prefixes.
