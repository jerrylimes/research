# Errata 6472 - RFC 8175

- **RFC Title:** Dynamic Link Exchange Protocol (DLEP)
- **RFC Publication Date:** June 2017

```
Section 12.4, para 2 says:


A Peer Offer Signal MUST be encoded within a UDP packet.  The IP source and destination fields in the packet MUST be set by swapping the values received in the Peer Discovery Signal.  The Peer Offer Signal completes the discovery process; see Section 7.1.

// state how to fix the above text here

```

## Issue description

The original text describes swapping IP source and destination addresses without specifying how to handle the source address in the Peer Offer Signal, resulting in an invalid packet.
