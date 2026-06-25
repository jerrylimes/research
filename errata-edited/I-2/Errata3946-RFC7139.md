# Errata 3946 - RFC 7139

- **RFC Title:** GMPLS Signaling Extensions for Control of Evolving G.709 Optical Transport Networks
- **RFC Publication Date:** March 2014

```
Section 7 says:


After decreasing the bandwidth, the ingress node

SHOULD send a ResvErr message to tear down the old control state.

// state how to fix the above text here

```

## Issue description

The message type used to tear down the old control state after decreasing bandwidth is incorrect. This inconsistency creates ambiguity in implementation.
