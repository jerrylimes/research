# Errata 5342 - RFC 83

- **RFC Title:** Protocol Independent Multicast - Sparse Mode (PIM-SM): Protocol Specification (Revised)
- **RFC Publication Date:** March 2016
- Link to original errata report: [rfc-editor.org/errata/eid5342](https://www.rfc-editor.org/errata/eid5342)

```
Section 4.4.2 says:


set KeepaliveTimer(S,G) to RP_Keepalive_Period;

// state how to fix the above text here

```

## Issue description

Setting the keepalive period for KAT(S, G) to RP_Keepalive_Period, which may be shorter than the actual keepalive period, can cause RP to time out the (S, G) state before the next Null-Register arrives. This inconsistency can lead to premature timeouts.
