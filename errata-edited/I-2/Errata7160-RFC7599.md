# Errata 7160 - RFC 7599

- **RFC Title:** Mapping of Address and Port using Translation (MAP-T)
- **RFC Publication Date:** July 2015

```
Section 10.1 says:


Translating an IPv4 packet to carry it across the MAP domain will increase its size (typically by 20 bytes).

// state how to fix the above text here

```

## Issue description

The original text does not fully consider what the size of the packet could possibly be. This inconsistency would lead to incorrect calculations of the size of translated packets.
