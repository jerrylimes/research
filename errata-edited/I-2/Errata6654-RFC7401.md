# Errata 6654 - RFC 7401

- **RFC Title:** Host Identity Protocol Version 2 (HIPv2)
- **RFC Publication Date:** April 2015

```
Section 5.3.3 says:


   If present in the I1 packet, the Initiator MUST include an unmodified

   copy of the R1_COUNTER parameter received in the corresponding R1

   packet into the I2 packet.

// state how to fix the above text here

```

## Issue description

The condition in the original text does not correctly identify which packet the Initiator should be present in. This inconsistency affects the implementation of the HIPv2 protocol.
