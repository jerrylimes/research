# Errata 6289 - RFC 8231

- **RFC Title:** Path Computation Element Communication Protocol (PCEP) Extensions for Stateful PCE
- **RFC Publication Date:** September 2017
- Link to original errata report: [rfc-editor.org/errata/eid6289](https://www.rfc-editor.org/errata/eid6289)

```
Section 7.3.2 says:


   Length (16 bits): indicates the total length of the TLV in octets and

   MUST be greater than 0.  The TLV MUST be zero-padded so that the TLV

   is 4-octet aligned.

// state how to fix the above text here

```

## Issue description

The way the original text defines the Length field is inconsistent with RFC 5440's TLV formatting in PCEP.
