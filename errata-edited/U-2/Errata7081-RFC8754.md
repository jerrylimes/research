# Errata 7081 - RFC 8754

- **RFC Title:** IPv6 Segment Routing Header (SRH)
- **RFC Publication Date:** March 2020
- Link to original errata report: [rfc-editor.org/errata/eid7081](https://www.rfc-editor.org/errata/eid7081)

```
Section 4.1.1 says:


A reduced SRH does not contain the first segment of the related SR

Policy (the first segment is the one already in the DA of the IPv6

header), and the Last Entry field is set to n-2, where n is the

number of elements in the SR Policy.

// state how to fix the above text here

```

## Issue description

The original text does not address the case where an SRH contains only one segment and TLVs. This inconsistency would lead to implementations incorrectly handling reduced SRHs with only one segment and TLVs.
