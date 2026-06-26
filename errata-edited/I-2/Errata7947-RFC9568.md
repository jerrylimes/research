# Errata 7947 - RFC 9568

- **RFC Title:** Virtual Router Redundancy Protocol (VRRP) Version 3 for IPv4 and IPv6
- **RFC Publication Date:** April 2024

```
Section 6.4.1 says:


         o  For each IPv4 address associated with the Virtual Router,

            broadcast a gratuitous ARP message containing the Virtual

            Router MAC address and with the target link-layer address

            set to the Virtual Router MAC address.

// state how to fix the above text here

```

## Issue description

The original text uses the wrong type of address in the gratuitous ARP message. This inconsistency would lead to implementations generating incorrect gratuitous ARP messages.
