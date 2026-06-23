# Errata 7639 - RFC 8029

- **RFC Title:** Detecting Multiprotocol Label Switched (MPLS) Data-Plane Failures
- **RFC Publication Date:** March 2017
- Link to original errata report: [rfc-editor.org/errata/eid7639](https://www.rfc-editor.org/errata/eid7639)

```
Section 4.5 says:


If the Reply Mode in the echo request is "Reply via an

IPv4 UDP packet with Router Alert", then the IP header MUST contain

the Router Alert IP Option of value 0x0 [RFC2113] for IPv4 or 69

[RFC7506] for IPv6.

// state how to fix the above text here

```

## Issue description

The original text is missing a packet type. This omission creates an inconsistency between the description and the broader functionality.
