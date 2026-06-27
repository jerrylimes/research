# Errata 4725 - RFC 7574

- **RFC Title:** Peer-to-Peer Streaming Peer Protocol (PPSPP)
- **RFC Publication Date:** July 2015

```
Section 5 says:


PPSPP can use different methods for protecting the integrity of the

content while it is being distributed via the peer-to-peer network.

More specifically, PPSPP can use different methods for receiving

peers to detect whether a requested chunk has been maliciously

modified by the sending peer. In benign environments, content

integrity protection can be disabled.



For static content, PPSPP currently defines one method for protecting

integrity, called the Merkle Hash Tree scheme. If PPSPP operates

over the Internet, this scheme MUST be used. If PPSPP operates in a

benign environment, this scheme MAY be used. So the scheme is

mandatory to implement, to satisfy the requirement of strong security

for an IETF protocol [RFC3365]. An extended version of the scheme is

used to efficiently protect dynamically generated content (live

streams), as explained below and in Section 6.1.

// state how to fix the above text here

```

## Issue description

The original text makes contradictory claims about whether content integrity protection is required, simultaneously permitting it to be disabled in certain environments and asserting that the scheme is mandatory to implement.

**For this example, the correct fix has been provided to you as a guide to how to correctly disambiguate the erroneous text.**

## Correct fix

```
It should say:

PPSPP can use different methods for protecting the integrity of the

content while it is being distributed via the peer-to-peer network.

More specifically, PPSPP can use different methods for receiving

peers to detect whether a requested chunk has been maliciously

modified by the sending peer.



For static content, PPSPP currently defines one method for protecting

integrity, called the Merkle Hash Tree scheme.

The scheme is mandatory to implement, to satisfy the requirement of

strong security for an IETF protocol [RFC3365]. An extended version

of the scheme is used to efficiently protect dynamically generated

content (live streams), as explained below and in Section 6.1.

```
