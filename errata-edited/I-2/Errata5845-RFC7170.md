# Errata 5845 - RFC 7170

- **RFC Title:** Tunnel Extensible Authentication Protocol (TEAP) Version 1
- **RFC Publication Date:** May 2014

```
Section 3.3.1 says:


   EAP method messages are carried within EAP-Payload TLVs defined in

   Section 4.2.10.  If more than one method is going to be executed in

   the tunnel, then upon method completion, the server MUST send an

   Intermediate-Result TLV indicating the result.

// state how to fix the above text here

```

## Issue description

The errata clarifies the use of Intermediate-Result TLVs. The original text in section 3.3.1 is not in sync with what the other sections and examples are suggesting.
