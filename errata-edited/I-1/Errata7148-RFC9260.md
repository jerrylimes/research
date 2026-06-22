# Errata 7148 - RFC 9260

- **RFC Title:** Stream Control Transmission Protocol
- **RFC Publication Date:** June 2022
- Link to original errata report: [rfc-editor.org/errata/eid7148](https://www.rfc-editor.org/errata/eid7148)

```
Section 3.3.3 says:


A receiver of an INIT ACK chunk with the a_rwnd value set to a

value smaller than 1500 MUST discard the packet, SHOULD send a

packet in response containing an ABORT chunk and using the

Initiate Tag as the Verification Tag, and MUST NOT change the

state of any existing association.

// state how to fix the above text here

```

## Issue description

The original specification for handling an INIT ACK chunk is inconsistent with the handling of other error conditions. It should align with the handling with other error conditions, ensuring consistent behavior across different scenarios.
