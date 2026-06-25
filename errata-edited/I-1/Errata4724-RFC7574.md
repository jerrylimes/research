# Errata 4724 - RFC 7574

- **RFC Title:** Peer-to-Peer Streaming Peer Protocol (PPSPP)
- **RFC Publication Date:** July 2015

```
Section 1.3 says:


swarm ID

Unique identifier for a swarm of peers, in PPSPP a sequence of

bytes. For video on demand with content integrity protection

enabled, the identifier is the so-called root hash of a Merkle

hash tree over the content. For live streaming, the swarm ID is

a public key.

// state how to fix the above text here
```

## Issue description

The swarm ID definition in Section 1.3 of RFC 7574 includes a qualifier that is inconsistent with how swarm IDs are treated in Sections 5 and 6.1, leaving the definition ambiguous for scenarios not covered by that qualifier.
