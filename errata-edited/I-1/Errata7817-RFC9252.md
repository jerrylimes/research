# Errata 7817 - RFC 9252

- **RFC Title:** BGP Overlay Services Based on Segment Routing over IPv6 (SRv6)
- **RFC Publication Date:** July 2022

```
Section 3.2.1 says:


   As defined in [RFC8986], the sum of the Locator Block Length (LBL),

   Locator Node Length (LNL), Function Length (FL), and Argument Length

   (AL) fields MUST be less than or equal to 128 and greater than the

   sum of Transposition Offset and Transposition Length.

// state how to fix the above text here

```

## Issue description

The original text's specification on the field length overlooks a possibility according to the text in that same section.
