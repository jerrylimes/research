# Errata 7804 - RFC 9463

- **RFC Title:** DHCP and Router Advertisement Options for the Discovery of Network-designated Resolvers (DNR)
- **RFC Publication Date:** November 2023

```
Section 6.1 says:


Note that the "Addr Length", "ipv6-address(es)", and "Service 

Parameters (SvcParams)" fields are not present if the ADN-only mode 

is used (Section 3.1.6).

// state how to fix the above text here

```

## Issue description

The original text incorrectly states that only "Addr Length", "ipv6-address(es)", and "Service Parameters (SvcParams)" fields are absent in ADN-only mode. This omission creates an inconsistency between the description in Section 6.1 and the actual specification of the ADN-only mode, directly impacting implementation.
