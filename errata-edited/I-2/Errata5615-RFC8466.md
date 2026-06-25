# Errata 5615 - RFC 8466

- **RFC Title:** A YANG Data Model for Layer 2 Virtual Private Network (L2VPN) Service Delivery
- **RFC Publication Date:** October 2018

```
Section 5.10.1 says:


   The svc-bandwidth parameter must include a "cos-id" parameter if the

   "type" is set to "bw-per-cos".  The cos-id can be assigned based on

   either (1) the IEEE 802.1p value [IEEE-802-1D] in the C-tag or

   (2) the Differentiated Services Code Point (DSCP) in the Ethernet

   frame header.  Service frames are metered against the bandwidth

   profile based on the cos-id.

// state how to fix the above text here

```

## Issue description

The original text does not correctly identify where the DSCP value is located. This inconsistency would affect implementations that incorrectly attempt to extract the DSCP value from the Ethernet header.
