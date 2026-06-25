# Errata 6938 - RFC 8013

- **RFC Title:** Forwarding and Control Element Separation (ForCES) Inter-FE Logical Functional Block (LFB)
- **RFC Publication Date:** February 2017

```
Section 5.1.1 says:


Caution needs to be exercised on how low the resulting reported link MTU could be: for IPv4 packets, the minimum size is 64 octets [RFC791] and for IPv6 the minimum size is 1280 octets [RFC2460].

// state how to fix the above text here

```

## Issue description

The original text incorrectly states the minimum MTU size for IPv4 packets. This inconsistency would mislead implementations calculating or interpreting the reported link MTU.
