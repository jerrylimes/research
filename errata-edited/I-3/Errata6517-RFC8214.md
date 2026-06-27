# Errata 6517 - RFC 8214

- **RFC Title:** Virtual Private Wire Service Support in Ethernet VPN
- **RFC Publication Date:** August 2017

```
Section 5 says:


   Finally, EVPN may employ data-plane egress link protection mechanisms

   not available in VPWS.  This can be done by the primary PE (on local

   AC down) using the label advertised in the per-EVI Ethernet A-D route

   by the backup PE to encapsulate the traffic and direct it to the

   backup PE.

// state how to fix the above text here

```

## Issue description

The original text fails to acknowledge the existence of data-plane egress link protection mechanisms in LDP-signaled PWs. The original text's factual inaccuracy makes it inconsistent.
