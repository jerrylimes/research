# Errata 5021 - RFC 7788

- **RFC Title:** Home Networking Control Protocol
- **RFC Publication Date:** April 2016
- Link to original errata report: [rfc-editor.org/errata/eid5021](https://www.rfc-editor.org/errata/eid5021)

```
Section says:

HNCP uses opaque 32-bit node identifiers

(DNCP_NODE_IDENTIFIER_LENGTH = 32).

// state how to fix the above text here

```

## Issue description

The original text presents a contradiction with Section 9's definition of the DNCP_NODE_IDENTIFIER_LENGTH field. This inconsistency creates a conflict between the two specifications, leading to potential incompatibility between implementations.
