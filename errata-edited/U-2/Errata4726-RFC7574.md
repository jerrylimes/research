# Errata 4726 - RFC 7574

- **RFC Title:** Peer-to-Peer Streaming Peer Protocol (PPSPP)
- **RFC Publication Date:** July 2015

```
Section 6.1 says:


In the "Unified Merkle Tree" method, PPSPP combines the Merkle Hash

Tree scheme for static content with signatures to unify the video-on-

demand and live streaming scenarios. The use of Merkle hash trees

reduces the number of signing and verification operations, hence

providing a similar signature amortization to the approach described

in [SIGMCAST]. If PPSPP operates over the Internet, the "Unified

Merkle Tree" method MUST be used. If the protocol operates in a

benign environment, the "Unified Merkle Tree" method MAY be used. So

this method is mandatory to implement.

// state how to fix the above text here

```

## Issue description

The original text makes contradictory claims about whether content integrity protection is required, simultaneously permitting it to be disabled in certain environments and asserting that the scheme is mandatory to implement.
