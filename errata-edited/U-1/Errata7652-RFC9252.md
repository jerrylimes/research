# Errata 7652 - RFC 9252

- **RFC Title:** BGP Overlay Services Based on Segment Routing over IPv6 (SRv6)
- **RFC Publication Date:** July 2022

```
Section 3.2.1 says:


   Transposition Offset indicates the bit position, and Transposition

   Length indicates the number of bits that are being taken out of the

   SRv6 SID value and encoded in the MPLS Label field.  The bits that

   have been shifted out MUST be set to 0 in the SID value.

// state how to fix the above text here

```

## Issue description

The original description of Transposition Offset and Transposition Length is unclear about the treatment of the extracted bits within the MPLS Label field, which is inconsistent with descriptions in Section 5 and 6, and creates confusion among readers.
